<main
  class="flex min-h-screen flex-row items-center justify-center gap-52 bg-red-300"
>
  <!-- Player 1 -->
  <section class="flex flex-col gap-7">
    <img
      src="/user-profile.svg"
      alt="User profile"
      class="h-60 w-60 self-center rounded-full border-2 border-black bg-white"
    />
    <span class="border-2 border-black bg-white p-2">Username</span>
    <button
      class="rounded-full border-2 border-black bg-blue-500 px-10 py-3 text-lg hover:bg-blue-600"
      >Heads</button
    >
  </section>

  <!-- Game UI -->
  <section class="flex flex-col justify-between gap-36 text-center">
    <h1 class="text-5xl">0 ICP</h1>
    <h2 class="text-2xl">Who will win?</h2>
    <div class="flex flex-row gap-10">
      <form action="/play" method="get">
        <button
          class="rounded-full border-2 border-black bg-purple-500 px-10 py-3 text-lg hover:bg-purple-600"
          >Play again!</button
        >
      </form>
      <a
        href="/home"
        class="rounded-full border-2 border-black bg-purple-500 px-10 py-3 text-lg hover:bg-purple-600"
        >Quit</a
      >
    </div>
  </section>

  <!-- Player 2 -->
  <section class="flex flex-col gap-7">
    <img
      src="/user-profile.svg"
      alt="User profile"
      class="h-60 w-60 self-center rounded-full border-2 border-black bg-white"
    />
    <span class="border-2 border-black bg-white p-2">Username</span>
    <button
      class="rounded-full border-2 border-black bg-red-500 px-10 py-3 text-lg hover:bg-red-600"
      >Tails</button
    >
  </section>
</main>
