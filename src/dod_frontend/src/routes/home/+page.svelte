<main
  class="grid min-h-screen min-w-full grid-flow-row grid-cols-4 grid-rows-12 gap-x-16 gap-y-5 bg-red-300 p-10"
>
  <!-- Profile sidebar -->
  <aside class="col-start-1 row-span-6 row-start-1 flex flex-col gap-16">
    <img
      src="user-profile.svg"
      alt="User profile"
      class="h-60 w-60 self-center rounded-full border-2 border-black bg-white"
    />
    <form action="post">
      <div class="flex flex-col gap-2">
        <input
          type="text"
          class="border-2 border-black bg-white p-2"
          value="Username Placeholder"
        />
        <button
          type="submit"
          class="max-w-fit rounded-full border-2 border-black bg-purple-500 px-10 py-3 hover:bg-purple-600"
          >Save username</button
        >
      </div>
    </form>
  </aside>

  <!-- Stats -->
  <h1 class="col-start-2 row-start-1 text-7xl font-bold">Stats</h1>
  <!-- First row -->
  <p class="relative col-start-2 row-start-2 text-lg">
    Games played: <span
      class="absolute inset-x-0 bottom-0 border-2 border-black bg-white p-2"
      >0</span
    >
  </p>
  <p class="relative col-start-3 row-start-2 text-lg">
    Games won: <span
      class="absolute inset-x-0 bottom-0 border-2 border-black bg-white p-2"
      >0</span
    >
  </p>
  <p class="relative col-start-4 row-start-2 text-lg">
    Win percentage: <span
      class="absolute inset-x-0 bottom-0 border-2 border-black bg-white p-2"
      >0%</span
    >
  </p>
  <!-- Second row -->
  <p class="relative col-start-2 row-start-4 text-lg">
    Winnings: <span
      class="absolute inset-x-0 bottom-0 border-2 border-black bg-white p-2"
      >0</span
    >
  </p>
  <p class="relative col-start-3 row-start-4 text-lg">
    Losses: <span
      class="absolute inset-x-0 bottom-0 border-2 border-black bg-white p-2"
      >0</span
    >
  </p>
  <p class="relative col-start-4 row-start-4 text-lg">
    Absolute: <span
      class="absolute inset-x-0 bottom-0 border-2 border-black bg-white p-2"
      >0</span
    >
  </p>

  <!-- Balance -->
  <p class="relative col-start-4 row-start-1 text-lg">
    Balance: <span
      class="absolute inset-x-0 bottom-0 border-2 border-black bg-white p-2"
      >0 ICP</span
    >
  </p>

  <!-- Actions -->
  <h1 class="col-start-2 row-start-6 text-7xl font-bold">Actions</h1>
  <div class="col-start-2 row-start-7 flex flex-row justify-between">
    <form action="play" method="post">
      <button
        class="rounded-full border-2 border-black bg-purple-500 px-10 py-3 text-lg hover:bg-purple-600"
        >Play!</button
      >
    </form>
    <form action="send">
      <button
        type="submit"
        class="rounded-full border-2 border-black bg-blue-500 px-10 py-3 text-lg hover:bg-blue-600"
        >Send balance</button
      >
    </form>
    <form action="logout">
      <button
        type="submit"
        class="rounded-full border-2 border-black bg-gray-500 px-10 py-3 text-lg hover:bg-gray-600"
        >Logout</button
      >
    </form>
  </div>
</main>
