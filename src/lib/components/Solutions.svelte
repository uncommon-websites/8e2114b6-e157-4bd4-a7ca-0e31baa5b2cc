<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
  import SolutionBlock from './SolutionBlock.svelte';
</script>

<SectionWrapper withBorderBottom={true} className="">
  <div class="px-4 md:px-12">
    <div class="py-16 text-center">
      <h2 class="font-serif text-4xl text-gray-900">How Lassie works</h2>
    </div>

    <!-- Block 1 -->
    <SolutionBlock
      label="Automated Insurance Posting"
      title="Post EOBs in seconds, not hours"
      description="Lassie automatically captures insurance payments from all major carriers and posts them directly to your practice management system. No more manual data entry, no more errors, no more wasted staff time."
    >
      <!-- Visual for Block 1: Insurance Documents -->
      <div class="relative w-full h-full flex items-center justify-center">
        <!-- Central Hub -->
        <div class="w-16 h-16 bg-white shadow-lg rounded-lg flex items-center justify-center z-10 border border-gray-100">
           <div class="w-8 h-8 bg-blue-600 rounded-sm"></div>
        </div>
        
        <!-- Connected Insurance Documents -->
        <div class="absolute top-1/4 left-1/4 bg-white p-3 shadow rounded border border-gray-100 animate-pulse">
            <div class="w-8 h-10 bg-blue-100 rounded flex items-center justify-center text-[10px] font-bold text-blue-700">EOB</div>
            <div class="mt-1 text-[10px] text-center">Delta</div>
        </div>
        <div class="absolute top-1/4 right-1/4 bg-white p-3 shadow rounded border border-gray-100">
            <div class="w-8 h-10 bg-blue-800 rounded flex items-center justify-center text-[10px] font-bold text-white">ERA</div>
            <div class="mt-1 text-[10px] text-center">BCBS</div>
        </div>
        <div class="absolute bottom-1/4 left-1/3 bg-white p-3 shadow rounded border border-gray-100">
            <div class="w-8 h-10 bg-blue-500 rounded flex items-center justify-center text-[10px] font-bold text-white">CHK</div>
            <div class="mt-1 text-[10px] text-center">MetLife</div>
        </div>
         <div class="absolute bottom-1/4 right-1/3 bg-white p-3 shadow rounded border border-gray-100">
            <div class="w-8 h-10 bg-gray-200 rounded flex items-center justify-center text-[10px] font-bold text-gray-600">EFT</div>
            <div class="mt-1 text-[10px] text-center">Cigna</div>
        </div>
        
        <!-- Connecting Lines -->
        <svg class="absolute inset-0 w-full h-full pointer-events-none opacity-20" viewBox="0 0 400 300">
            <path d="M100 100 L200 150 M300 100 L200 150 M150 220 L200 150 M250 220 L200 150" stroke="currentColor" stroke-width="1" stroke-dasharray="4 4" />
        </svg>
      </div>
    </SolutionBlock>

    <!-- Block 2 -->
    <SolutionBlock
      label="Payment Reconciliation"
      title="Match payments automatically"
      description="Lassie reconciles every insurance payment with outstanding claims in your PMS. See exactly what was paid, what's pending, and what needs follow-up—all in one place. Reduce your accounts receivable by up to 75%."
      reversed={true}
    >
      <!-- Visual for Block 2: Payment Dashboard -->
      <div class="bg-white rounded-lg shadow-xl p-6 w-3/4 max-w-sm border border-gray-100">
        <div class="flex items-center space-x-3 mb-4">
            <div class="w-8 h-8 rounded-full bg-blue-600 flex items-center justify-center text-white text-xs font-bold">
                $
            </div>
            <div class="text-xs text-gray-500">Payment Reconciliation</div>
        </div>
        <h4 class="font-serif text-xl mb-4">Today's Payments</h4>
        <div class="space-y-3 mb-6">
            <div class="flex justify-between items-center p-2 bg-green-50 rounded">
                <span class="text-xs text-gray-700">Delta Dental</span>
                <span class="text-xs font-bold text-green-700">$2,450</span>
            </div>
            <div class="flex justify-between items-center p-2 bg-green-50 rounded">
                <span class="text-xs text-gray-700">BCBS</span>
                <span class="text-xs font-bold text-green-700">$1,890</span>
            </div>
            <div class="flex justify-between items-center p-2 bg-blue-50 rounded">
                <span class="text-xs text-gray-700">MetLife</span>
                <span class="text-xs font-bold text-blue-700">Pending</span>
            </div>
        </div>
        <button class="w-full bg-blue-700 text-white py-2 rounded text-sm font-medium flex items-center justify-center space-x-2">
            <span>View Full Report</span>
            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3"></path></svg>
        </button>
      </div>
    </SolutionBlock>

    <!-- Block 3 -->
    <SolutionBlock
      label="Concierge Support"
      title="Your dedicated posting team"
      description="Get personal support from posting experts who work as an extension of your practice. Available via WhatsApp, phone, and email, our team ensures every payment is posted accurately and on time."
    >
       <!-- Visual for Block 3: Support Card -->
       <div class="bg-white rounded shadow-lg p-8 w-2/3 max-w-xs border border-gray-100 relative">
          <div class="flex justify-between items-center mb-6 border-b pb-2">
              <div class="font-bold text-xs">Lassie Support</div>
              <div class="w-4 h-4 bg-green-500 rounded-full"></div>
          </div>
          <div class="mb-4">
              <h5 class="font-bold text-sm">Your Practice Advisor</h5>
              <div class="text-[10px] text-gray-400">Available via WhatsApp, phone & email</div>
          </div>
          <div class="space-y-3 text-[10px] text-gray-600 leading-relaxed">
              <div class="flex items-start gap-2">
                  <div class="w-1 h-1 bg-blue-600 rounded-full mt-1.5"></div>
                  <p>Personal responses from posting experts</p>
              </div>
              <div class="flex items-start gap-2">
                  <div class="w-1 h-1 bg-blue-600 rounded-full mt-1.5"></div>
                  <p>Multi-channel accessibility</p>
              </div>
              <div class="flex items-start gap-2">
                  <div class="w-1 h-1 bg-blue-600 rounded-full mt-1.5"></div>
                  <p>Works as part of your team</p>
              </div>
          </div>
       </div>
    </SolutionBlock>
  </div>
</SectionWrapper>
