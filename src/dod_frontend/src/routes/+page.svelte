<script lang="ts">
  import { AuthClient } from "@dfinity/auth-client";
  import { onMount } from "svelte";

  onMount(async () => {
    const identityProvider =
      process.env.DFX_NETWORK === "local"
        ? "http://be2us-64aaa-aaaaa-qaabq-cai.localhost:4943/"
        : "identity.ic0.app";

    const loginButton = document.getElementById(
      "login-button",
    ) as HTMLButtonElement;
    loginButton.onclick = async (e) => {
      e.preventDefault();
      const authClient = await AuthClient.create();
      await new Promise<void>((resolve, reject) => {
        authClient.login({
          onSuccess: () => {
            console.log("Logged in");
            location.href = "/home";
            resolve();
          },
          onError: reject,
          identityProvider,
        });
      });
    };
  });
</script>

<main
  class="flex min-h-screen min-w-full flex-col items-center justify-center gap-20 bg-red-300"
>
  <div class="grid grid-cols-3 grid-rows-3 gap-10">
    <span class="col-span-2 col-start-1 row-start-1 text-9xl">Double</span>
    <span class="col-start-2 row-start-2 text-center text-9xl">or</span>
    <span class="col-span-2 col-start-2 row-start-3 text-right text-9xl"
      >Done</span
    >
  </div>
  <button
    id="login-button"
    class="rounded-full border-2 border-black bg-purple-500 px-10 py-3 text-5xl hover:bg-purple-600"
    >Login!</button
  >
</main>
