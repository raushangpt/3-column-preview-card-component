<script>
  let cards = [
    [
      './images/icon-sedans.svg',
      'Sedans',
      'Choose a sedan for its affordability and excellent fuel economy. Ideal for cruising in the city or on your next road trip.',
      'clr01',
    ],
    [
      './images/icon-suvs.svg',
      'SUVs',
      'Take an SUV for its spacious interior, power, and versatility. Perfect for your next family vacation and off-road adventures.',
      'clr02',
    ],
    [
      './images/icon-luxury.svg',
      'Luxury',
      'Cruise in the best car brands without the bloated prices. Enjoy the enhanced comfort of a luxury rental and arrive in style',
      'clr03',
    ],
  ];
</script>

<div
  class="bg-very-light-gray grid min-h-screen w-screen place-items-center p-20">
  <div
    class="font-lexend-deca max-w-xs overflow-hidden rounded-xl shadow-xl transition-all hover:shadow-2xl sm:max-w-sm lg:grid lg:max-w-screen-lg lg:grid-cols-3">
    {#each cards as [src, title, para, clr]}
      <div
        class="{clr} space-y-6 p-6 sm:p-10 lg:flex lg:flex-col lg:justify-between lg:p-14">
        <div class="space-y-6">
          <img {src} alt="" />

          <h1
            class="font-big-shoulders-display text-very-light-gray text-4xl uppercase">
            {title}
          </h1>

          <p class="text-transparent-white lg:pb-16">
            {para}
          </p>
        </div>

        <div class="">
          <button
            class="bg-very-light-gray hover:text-very-light-gray rounded-full px-8 py-3 hover:bg-[#111]">
            Learn More
          </button>
        </div>
      </div>
    {/each}
  </div>
</div>

<style>
  .clr01 {
    @apply bg-bright-orange;
  }

  .clr02 {
    @apply bg-dark-cyan;
  }

  .clr03 {
    @apply bg-very-dark-cyan;
  }
</style>
