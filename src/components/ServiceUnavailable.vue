<script setup>
const contactEmail = 'dev-support@devconnect.com'
const reloadPage = () => window.location.reload()
</script>

<template>
  <div class="w-full flex items-center justify-center">
    <div class="max-w-screen-xl w-full">
      <div class="rounded-2xl border border-slate-200 bg-white shadow-xl overflow-hidden transition-all duration-300 max-h-[90vh] flex flex-col">
        <div class="flex flex-col lg:flex-row overflow-y-auto lg:overflow-visible">
          <!-- Left: Illustration/Icon Section -->
          <div class="lg:w-2/3 xl:w-2/5 bg-slate-50 flex flex-col items-center justify-center p-6 sm:p-10 border-b lg:border-b-0 lg:border-r border-slate-200 flex-shrink-0">
            <div class="relative group">
              <div class="absolute -inset-4 bg-red-100 rounded-full blur-xl opacity-30 group-hover:opacity-50 transition-opacity animate-pulse"></div>
              <div class="relative p-6 sm:p-8 bg-white rounded-full shadow-md border border-slate-100 transform transition-transform group-hover:scale-105">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-16 w-16 sm:h-24 sm:w-24 text-red-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.25" d="M12 9v2m0 4h.01m-6.938 4h13.856c1.54 0 2.502-1.667 1.732-3L13.732 4c-.77-1.333-2.694-1.333-3.464 0L3.34 16c-.77 1.333.192 3 1.732 3z" />
                </svg>
              </div>
            </div>
            <div class="mt-6 text-center">
              <span class="inline-flex items-center px-3 py-1 rounded-full text-xs font-bold bg-red-50 text-red-700 border border-red-100 shadow-sm">
                Status: 503
              </span>
              <p class="mt-3 text-slate-400 text-[10px] sm:text-xs font-bold uppercase tracking-[0.2em]">Maintenance Mode</p>
            </div>
          </div>

          <!-- Right: Content Section -->
          <div class="lg:w-2/3 xl:w-3/5 p-6 sm:p-10 lg:p-16 flex flex-col justify-center bg-white overflow-y-auto">
            <div class="max-w-2xl">
              <h1 class="text-3xl sm:text-4xl xl:text-5xl font-black text-slate-900 tracking-tight leading-tight mb-4 sm:mb-6">
                We'll be <br class="hidden sm:block" />
                <span class="text-red-600">Back Soon</span>
              </h1>
              
              <p class="text-base sm:text-lg text-slate-600 mb-6 sm:mb-8 leading-relaxed font-medium">
                Essential maintenance is underway. We're working hard to get back as quickly as possible.
              </p>

              <div class="grid gap-4 sm:gap-6 mb-8 sm:mb-10">
                <div class="flex items-start gap-4 p-4 sm:p-5 rounded-xl bg-slate-50 border border-slate-100">
                  <div class="flex-shrink-0 p-2 bg-white rounded-lg shadow-sm border border-slate-100">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-slate-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
                    </svg>
                  </div>
                  <div>
                    <h4 class="text-sm font-bold text-slate-800">Why the wait?</h4>
                    <p class="text-xs sm:text-sm text-slate-500 mt-1 leading-relaxed">Server is offline for scheduled updates to ensure data safety.</p>
                  </div>
                </div>

                <div class="flex flex-col sm:flex-row gap-4">
                  <a 
                    :href="`mailto:${contactEmail}`"
                    class="group w-full sm:w-auto inline-flex items-center justify-center px-6 py-3 sm:px-8 sm:py-4 rounded-xl bg-slate-900 text-white text-sm font-bold hover:bg-slate-800 transition-all transform hover:-translate-y-1 active:scale-95 shadow-lg shadow-slate-200"
                  >
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-2 transition-transform group-hover:rotate-12" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                    </svg>
                    Contact Developer
                  </a>
                  <button 
                    @click="reloadPage"
                    class="w-full sm:w-auto px-6 py-3 sm:px-8 sm:py-4 rounded-xl border-2 border-slate-200 text-slate-700 text-sm font-bold hover:bg-slate-50 hover:border-slate-300 transition-all active:scale-95"
                  >
                    Try Again
                  </button>
                </div>
              </div>

              <div class="flex items-center gap-2 text-xs">
                <span class="flex h-2 w-2 rounded-full bg-orange-400 animate-pulse"></span>
                <span class="text-slate-400 font-bold uppercase tracking-wider">
                  Wait time: <span class="text-slate-900">15-30m</span>
                </span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
