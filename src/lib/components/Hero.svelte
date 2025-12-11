<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
</script>

<SectionWrapper withBorderBottom={true} className="py-20 md:py-24">
  <div class="px-4 md:px-12 max-w-4xl mx-auto text-center">
    <h1 class="font-serif text-5xl md:text-7xl text-gray-900 mb-6 leading-tight">
      Accelerate your dental <br/> practice cash flow
    </h1>
    <p class="text-gray-500 text-lg md:text-xl max-w-2xl mx-auto mb-10 leading-relaxed font-light">
      Free up 15 hours per week with automated insurance claim posting and payment reconciliation. Get paid up to 4x faster while your team focuses on patient care.
    </p>
    <a href="#" class="inline-flex items-center px-6 py-3 bg-[var(--color-primary-blue)] text-white font-medium rounded hover:opacity-90 transition-opacity">
      Schedule a Demo <span class="ml-2">→</span>
    </a>
  </div>

  <div class="mt-16 md:mt-20 px-4 md:px-12">
    <div class="relative w-full aspect-[16/9] md:aspect-[21/9] rounded-lg overflow-hidden bg-gray-200">
      <!-- Hero Image -->
      <img 
        src="/generated/image-dental-team-working-together-in-modern-d-1765490085103-0.webp" 
        alt="Dental team collaborating with Lassie" 
        class="w-full h-full object-cover"
      />
      
      <!-- Video Overlay Button -->
      <div class="absolute inset-0 flex items-center justify-center">
        <button class="flex items-center space-x-3 bg-black/80 backdrop-blur-sm text-white px-5 py-3 rounded hover:bg-black transition-colors">
          <svg class="w-4 h-4 fill-current" viewBox="0 0 24 24">
            <path d="M8 5v14l11-7z" />
          </svg>
          <span class="text-sm font-medium">See how Lassie transforms dental practices</span>
        </button>
      </div>
    </div>
  </div>
</SectionWrapper>
