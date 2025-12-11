<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
</script>

<SectionWrapper withBorderBottom={true} withBorderTop={true} className="py-6">
  <nav class="flex items-center justify-between px-4 md:px-12">
    <!-- Logo -->
    <div class="font-serif text-2xl font-medium tracking-wide">
      Lassie
    </div>

    <!-- Links -->
    <div class="hidden md:flex items-center space-x-8 text-sm text-gray-600 font-medium">
      <a href="#" class="hover:text-gray-900">Integrations</a>
      <a href="#" class="hover:text-gray-900">Customers</a>
      <a href="#" class="hover:text-gray-900">Events</a>
      <a href="#" class="hover:text-gray-900">Support</a>
    </div>

    <!-- Action -->
    <div>
      <a href="#" class="inline-block px-6 py-2 bg-gray-100 hover:bg-gray-200 text-gray-900 text-sm font-medium rounded transition-colors">
        Get Started
      </a>
    </div>
  </nav>
</SectionWrapper>
