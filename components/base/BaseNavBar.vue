<template>
  <nav class="fixed z-20 w-full bg-white">
    <!-- Base Navigation Bar For Desktop -->
    <div class="hidden lg:block">
      <BaseContainer class="my-30px justify-between">
        <div class="flex flex-row justify-center items-center">
          <a
            href="#"
            class="font-semibold text-24px-30px -tracking-0.2px text-primary mr-10 font-plus-jakarta-sans"
          >
            maket<span class="text-secondary">er.</span>
          </a>
          <div
            class="flex flex-row justify-center items-center space-x-9 font-general-sans font-medium text-18px-24px -tracking-0.5px"
          >
            <a
              href="#"
              class="transition duration-500 ease text-primary hover:text-primary"
            >
              Home
            </a>
            <a
              href="#"
              class="transition duration-500 ease text-dark hover:text-primary"
            >
              Job
            </a>
            <a
              href="#"
              class="transition duration-500 ease text-dark hover:text-primary"
            >
              Hiring
            </a>
            <a
              href="#"
              class="transition duration-500 ease text-dark hover:text-primary"
            >
              About
            </a>
            <BaseInput
              placeholder="Find marketer"
              class="relative w-200px"
              class-input="px-52px font-general-sans font-medium -tracking-0.6px text-16px-22px h-50px"
            >
              <div
                class="flex absolute inset-y-0 left-0 items-center pl-25px pointer-events-none"
              >
                <svg
                  width="16"
                  height="16"
                  viewBox="0 0 16 16"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <g clip-path="url(#clip0_1_82)">
                    <path
                      d="M14.6667 14.6667L13.3333 13.3334M7.66668 14C8.49838 14 9.32194 13.8362 10.0903 13.5179C10.8587 13.1997 11.5569 12.7332 12.145 12.145C12.7331 11.5569 13.1996 10.8588 13.5179 10.0904C13.8362 9.32197 14 8.49841 14 7.66671C14 6.835 13.8362 6.01144 13.5179 5.24305C13.1996 4.47465 12.7331 3.77647 12.145 3.18836C11.5569 2.60026 10.8587 2.13375 10.0903 1.81547C9.32194 1.49719 8.49838 1.33337 7.66668 1.33337C5.98697 1.33337 4.37606 2.00063 3.18833 3.18836C2.0006 4.37609 1.33334 5.987 1.33334 7.66671C1.33334 9.34641 2.0006 10.9573 3.18833 12.145C4.37606 13.3328 5.98697 14 7.66668 14Z"
                      stroke="#D9D9D9"
                      stroke-width="1.5"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                  </g>
                  <defs>
                    <clipPath id="clip0_1_82">
                      <rect width="16" height="16" fill="white" />
                    </clipPath>
                  </defs>
                </svg>
              </div>
            </BaseInput>
          </div>
        </div>
        <div class="flex flex-row justify-center items-center space-x-14px">
          <BaseButton color="primary" class="py-19px px-4 h-50px">
            <div
              class="flex flex-row justify-center items-center w-108px h-11px font-general-sans font-semibold text-16px-22px -tracking-0.6px"
            >
              Login
            </div>
          </BaseButton>
          <BaseButton color="secondary" class="py-19px px-4 h-50px">
            <div
              class="flex flex-row justify-center items-center w-108px h-11px font-general-sans font-semibold text-16px-22px -tracking-0.6px"
            >
              Register
            </div>
          </BaseButton>
        </div>
      </BaseContainer>
    </div>
  </nav>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped></style>
