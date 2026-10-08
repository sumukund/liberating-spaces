<script lang="ts">
    // import { goto } from '$app/navigation';
    // import { homepage } from '#lib/data/homepage';
</script>

<svelte:head>
    <title>Liberating Spaces</title>
</svelte:head>


  <div class="flex h-screen overflow-hidden">
    
    <!-- SIDEBAR: Hidden on mobile, fixed on desktop -->
    <aside class="hidden w-64 flex-col bg-cream-900 border-r border-cream-800 p-4 md:flex">
      <div class="flex items-center gap-2 px-2 py-3">
        <div class="h-8 w-8 rounded-lg bg-purple-600 flex items-center justify-center font-bold text-white">A</div>
        <span class="text-lg font-semibold tracking-tight">DashboardApp</span>
      </div>
      
      <nav class="mt-6 flex-1 space-y-1">
        <a href="#" class="flex items-center gap-3 rounded-lg bg-indigo-600/10 px-3 py-2 text-sm font-medium text-indigo-400">
          <span></span> Dashboard
        </a>
        <a href="#" class="flex items-center gap-3 rounded-lg px-3 py-2 text-sm font-medium text-slate-400 hover:bg-slate-800 hover:text-slate-200 transition-colors">
          <span></span> Projects
        </a>
        <a href="#" class="flex items-center gap-3 rounded-lg px-3 py-2 text-sm font-medium text-slate-400 hover:bg-slate-800 hover:text-slate-200 transition-colors">
          <span></span> Settings
        </a>
      </nav>
    </aside>

    <!-- MAIN VIEW AREA -->
    <div class="flex flex-1 flex-col overflow-y-auto bg-slate-950">
      
      <!-- TOP NAVIGATION BAR -->
      <header class="flex h-16 items-center justify-between border-b border-slate-800 bg-slate-900/50 px-6 backdrop-blur">
        <h1 class="text-xl font-bold">Overview</h1>
        <div class="flex items-center gap-4">
          <button class="rounded-full bg-slate-800 p-1 text-slate-400 hover:text-slate-200">
            <span class="sr-only">Notifications</span>🔔
          </button>
          <div class="h-8 w-8 rounded-full bg-slate-700 object-cover" aria-hidden="true"></div>
        </div>
      </header>

      <!-- MAIN APP CONTENT -->
      <main class="p-6">
        <!-- Stat Grid -->
        <div class="grid grid-cols-1 gap-6 sm:grid-cols-2 lg:grid-cols-3">
          
          <!-- Card 1 -->
          <div class="rounded-xl border border-slate-800 bg-slate-900 p-6 shadow-sm">
            <p class="text-sm font-medium text-slate-400">Total Revenue</p>
            <p class="mt-2 text-3xl font-semibold tracking-tight">$48,259.50</p>
            <span class="mt-2 inline-flex items-center text-xs font-medium text-emerald-400">↑ 12% from last month</span>
          </div>

          <!-- Card 2 -->
          <div class="rounded-xl border border-slate-800 bg-slate-900 p-6 shadow-sm">
            <p class="text-sm font-medium text-slate-400">Active Users</p>
            <p class="mt-2 text-3xl font-semibold tracking-tight">+10,342</p>
            <span class="mt-2 inline-flex items-center text-xs font-medium text-emerald-400">↑ 4.3% from last week</span>
          </div>

          <!-- Card 3 -->
          <div class="rounded-xl border border-slate-800 bg-slate-900 p-6 shadow-sm">
            <p class="text-sm font-medium text-slate-400">Server Uptime</p>
            <p class="mt-2 text-3xl font-semibold tracking-tight">99.98%</p>
            <span class="mt-2 inline-flex items-center text-xs font-medium text-slate-500">Stable</span>
          </div>
          
        </div>
      </main>
    </div>

  </div>

