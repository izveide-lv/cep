<template>
  <div
    class="relative flex items-center justify-center gap-10 before:h-px before:w-full before:border-b before:[border-image:linear-gradient(to_right,transparent,--theme(--color-indigo-300/.8),transparent)1] dark:before:[border-image:linear-gradient(to_right,transparent,--theme(--color-indigo-300/.16),transparent)1] before:shadow-xs before:shadow-white/20 dark:before:shadow-none after:h-px after:w-full after:border-b after:[border-image:linear-gradient(to_right,transparent,--theme(--color-indigo-300/.8),transparent)1] dark:after:[border-image:linear-gradient(to_right,transparent,--theme(--color-indigo-300/.16),transparent)1] after:shadow-xs after:shadow-white/20 dark:after:shadow-none mb-11"
  >
    <div class="w-full max-w-xs mx-auto shrink-0">
      <form class="relative" name="cep" action="/paldies" method="POST" netlify>
        <!-- Border with dots in corners -->
        <div
          class="absolute -inset-3 bg-indigo-500/15 dark:bg-transparent dark:bg-linear-to-b dark:from-gray-700/80 dark:to-gray-700/70 rounded-lg -z-10 before:absolute before:inset-y-0 before:left-0 before:w-[15px] before:bg-[length:15px_15px] before:[background-position:top_center,bottom_center] before:bg-no-repeat before:[background-image:radial-gradient(circle_at_center,--theme(--color-indigo-500/.56)_1.5px,transparent_1.5px),radial-gradient(circle_at_center,--theme(--color-indigo-500/.56)_1.5px,transparent_1.5px)] dark:before:[background-image:radial-gradient(circle_at_center,var(--color-gray-600)_1.5px,transparent_1.5px),radial-gradient(circle_at_center,var(--color-gray-600)_1.5px,transparent_1.5px)] after:absolute after:inset-y-0 after:right-0 after:w-[15px] after:bg-[length:15px_15px] after:[background-position:top_center,bottom_center] after:bg-no-repeat after:[background-image:radial-gradient(circle_at_center,--theme(--color-indigo-500/.56)_1.5px,transparent_1.5px),radial-gradient(circle_at_center,--theme(--color-indigo-500/.56)_1.5px,transparent_1.5px)] dark:after:[background-image:radial-gradient(circle_at_center,var(--color-gray-600)_1.5px,transparent_1.5px),radial-gradient(circle_at_center,var(--color-gray-600)_1.5px,transparent_1.5px)]"
          aria-hidden="true"
        ></div>

        <div class="space-y-3">
          <div>
            <label class="sr-only" for="email">E-pasts</label>
            <div class="relative">
              <div
                class="absolute inset-y-0 left-0 text-gray-500/70 dark:text-gray-400/70 pl-3 flex items-center pointer-events-none"
              >
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="icon icon-tabler icons-tabler-outline icon-tabler-mail"
                >
                  <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                  <path
                    d="M3 7a2 2 0 0 1 2 -2h14a2 2 0 0 1 2 2v10a2 2 0 0 1 -2 2h-14a2 2 0 0 1 -2 -2v-10z"
                  />
                  <path d="M3 7l9 6l9 -6" />
                </svg>
              </div>
              <input
                id="email"
                class="form-input text-sm w-full pl-10 pr-4"
                type="email"
                placeholder="Tavs e-pasts"
                required
              />
            </div>
          </div>
          <div>
            <label class="sr-only" for="email">E-pasts</label>
            <div class="relative">
              <div
                class="absolute inset-y-0 left-0 text-gray-500/70 dark:text-gray-400/70 pl-3 flex items-center pointer-events-none"
              >
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="icon icon-tabler icons-tabler-outline icon-tabler-world-www"
                >
                  <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                  <path
                    d="M19.5 7a9 9 0 0 0 -7.5 -4a8.991 8.991 0 0 0 -7.484 4"
                  />
                  <path d="M11.5 3a16.989 16.989 0 0 0 -1.826 4" />
                  <path d="M12.5 3a16.989 16.989 0 0 1 1.828 4" />
                  <path
                    d="M19.5 17a9 9 0 0 1 -7.5 4a8.991 8.991 0 0 1 -7.484 -4"
                  />
                  <path d="M11.5 21a16.989 16.989 0 0 1 -1.826 -4" />
                  <path d="M12.5 21a16.989 16.989 0 0 0 1.828 -4" />
                  <path d="M2 10l1 4l1.5 -4l1.5 4l1 -4" />
                  <path d="M17 10l1 4l1.5 -4l1.5 4l1 -4" />
                  <path d="M9.5 10l1 4l1.5 -4l1.5 4l1 -4" />
                </svg>
              </div>
              <input
                id="www"
                class="form-input text-sm w-full pl-10 pr-4"
                type="text"
                placeholder="Mājaslapas adrese"
                required
              />
            </div>
          </div>
          <div>
            <button
              class="btn text-gray-100 bg-gray-900 hover:bg-gray-800 dark:text-gray-800 dark:bg-gray-100 dark:hover:bg-white w-full cursor-pointer"
            >
              Saņemt novērtējumu
            </button>
          </div>
        </div>
      </form>
    </div>
  </div>

  <div class="max-w-3xl mx-auto">
    <div class="text-center">
      <p class="text-sm text-gray-500">
        Tavi dati ir
        <span class="text-gray-700 dark:text-gray-200 font-medium"
          >pilnīgā drošībā</span
        >
        un novērtējums
        <span class="text-gray-700 dark:text-gray-200 font-medium"
          >nebūs publisks</span
        >.
      </p>
    </div>
  </div>
</template>
