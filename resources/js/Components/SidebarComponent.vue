<script setup>
import { Link } from '@inertiajs/vue3';

defineProps({
    isCollapsed: Boolean
})
</script>

<template>
    <nav>
        <Link href="/dashboard" class="flex items-center space-x-2">
            <img src="https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/c15c4f2f-039f-48eb-8339-cad57b2b5353/da0373y-5e90f4d3-e020-4e2c-ad35-7bead062a572.jpg?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOjdlMGQxODg5ODIyNjQzNzNhNWYwZDQxNWVhMGQyNmUwIiwiaXNzIjoidXJuOmFwcDo3ZTBkMTg4OTgyMjY0MzczYTVmMGQ0MTVlYTBkMjZlMCIsIm9iaiI6W1t7InBhdGgiOiJcL2ZcL2MxNWM0ZjJmLTAzOWYtNDhlYi04MzM5LWNhZDU3YjJiNTM1M1wvZGEwMzczeS01ZTkwZjRkMy1lMDIwLTRlMmMtYWQzNS03YmVhZDA2MmE1NzIuanBnIn1dXSwiYXVkIjpbInVybjpzZXJ2aWNlOmZpbGUuZG93bmxvYWQiXX0.WHfdoujXOK7FXQm5ufsD1ADvOXyhpxlrJG1ofYhSy-g" alt="" class="w-[40px] rounded-sm shadow-sm border">
            <span v-show="!isCollapsed" class="text-2xl text-gray-600 font-extrabold">Altair Encina</span>
        </Link>
        <hr class="mt-3">

        <div class="flex flex-col space-y-3 mt-4" :class="{ 'items-center' : isCollapsed }">
            <Link href="/dashboard" class="px-2 py-1.5 rounded-lg text-gray-700 flex items-center space-x-2 hover:bg-gray-100">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6A2.25 2.25 0 016 3.75h2.25A2.25 2.25 0 0110.5 6v2.25a2.25 2.25 0 01-2.25 2.25H6a2.25 2.25 0 01-2.25-2.25V6zM3.75 15.75A2.25 2.25 0 016 13.5h2.25a2.25 2.25 0 012.25 2.25V18a2.25 2.25 0 01-2.25 2.25H6A2.25 2.25 0 013.75 18v-2.25zM13.5 6a2.25 2.25 0 012.25-2.25H18A2.25 2.25 0 0120.25 6v2.25A2.25 2.25 0 0118 10.5h-2.25a2.25 2.25 0 01-2.25-2.25V6zM13.5 15.75a2.25 2.25 0 012.25-2.25H18a2.25 2.25 0 012.25 2.25V18A2.25 2.25 0 0118 20.25h-2.25A2.25 2.25 0 0113.5 18v-2.25z" />
                  </svg>
                  
                <span v-show="!isCollapsed" class="text-base">Dashboard</span>
            </Link>
            <Link href="/clients" class="px-2 py-1.5 rounded-lg text-sm text-gray-700 flex items-center space-x-2 hover:bg-gray-100">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M20.25 14.15v4.25c0 1.094-.787 2.036-1.872 2.18-2.087.277-4.216.42-6.378.42s-4.291-.143-6.378-.42c-1.085-.144-1.872-1.086-1.872-2.18v-4.25m16.5 0a2.18 2.18 0 00.75-1.661V8.706c0-1.081-.768-2.015-1.837-2.175a48.114 48.114 0 00-3.413-.387m4.5 8.006c-.194.165-.42.295-.673.38A23.978 23.978 0 0112 15.75c-2.648 0-5.195-.429-7.577-1.22a2.016 2.016 0 01-.673-.38m0 0A2.18 2.18 0 013 12.489V8.706c0-1.081.768-2.015 1.837-2.175a48.111 48.111 0 013.413-.387m7.5 0V5.25A2.25 2.25 0 0013.5 3h-3a2.25 2.25 0 00-2.25 2.25v.894m7.5 0a48.667 48.667 0 00-7.5 0M12 12.75h.008v.008H12v-.008z" />
                  </svg>
                  
                <span v-show="!isCollapsed" class="text-sm">Clients</span>
            </Link>
        </div>
    </nav>
</template>