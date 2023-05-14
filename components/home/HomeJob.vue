<template>
  <div class="bg-alabaster mt-150px">
    <BaseContainer>
      <div class="mx-auto">
        <p
          class="mt-100px font-general-sans font-medium text-black text-48px-64px -tracking-0.01em text-center"
        >
          2000+ Job Openings
        </p>
        <p
          class="font-general-sans font-medium text-light text-18px-30px -tracking-0.01em text-center max-w-2xl mx-auto"
        >
          Explore thousand of marketing job opportunities and find your dream
          company with our comprehensive marketing job search platform
        </p>
        <div class="mt-9 grid lg:grid-cols-3 grid-cols-1 gap-8 w-full">
          <HomeJobCard class="flex-3"></HomeJobCard>
          <HomeJobCard class="flex-3"></HomeJobCard>
          <HomeJobCard class="flex-3"></HomeJobCard>
          <HomeJobCard class="flex-3"></HomeJobCard>
          <HomeJobCard class="flex-3"></HomeJobCard>
          <HomeJobCard class="flex-3"></HomeJobCard>
        </div>
        <BaseButton
          color="primary"
          class="py-19px px-4 h-50px mx-auto mt-8 mb-11"
        >
          <div
            class="flex flex-row justify-center items-center w-108px h-11px font-general-sans font-medium text-16px-22px -tracking-0.6px"
          >
            Load more
          </div>
        </BaseButton>
      </div>
    </BaseContainer>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped></style>
