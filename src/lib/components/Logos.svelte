<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
</script>

<SectionWrapper withBorderBottom={true} className="py-12">
  <div class="px-4 md:px-12 flex flex-col md:flex-row items-center justify-between gap-8">
    <!-- Logos -->
    <div class="flex flex-wrap items-center gap-8 md:gap-12 grayscale opacity-70">
        <!-- Delta Dental -->
        <div class="h-6 font-bold text-lg tracking-tight">DELTA DENTAL</div>
        <!-- Blue Cross Blue Shield -->
        <div class="h-8 flex flex-col leading-none text-xs font-bold uppercase tracking-wide">
            <span>BLUE CROSS</span>
            <span>BLUE SHIELD</span>
        </div>
        <!-- Dentrix -->
        <div class="h-6 font-bold text-lg italic">Dentrix</div>
        <!-- MetLife -->
        <div class="h-6 font-medium text-lg tracking-wide">
            MetLife
        </div>
    </div>

    <!-- Trust Text -->
    <div class="text-gray-400 text-sm font-light text-right md:text-left">
      Trusted by over 1,000 dental practices
    </div>
  </div>
</SectionWrapper>
