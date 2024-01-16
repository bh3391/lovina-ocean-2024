<template>
    <div  class="navbar bg-slate-100 ">
        <div class="navbar-start">
            <div class="dropdown">
                <label tabindex="0" class="btn btn-ghost ">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24"
                        stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h8m-8 6h16" />
                    </svg>
                </label>
                <ul tabindex="0"
                    class="menu menu-compact dropdown-content mt-3 p-2 shadow text-black rounded-box w-60 bg-slate-50">


                    <li>

                        <NuxtLink to="/about" class="link link-hover">About</NuxtLink>
                        <NuxtLink to="/contact" class="link link-hover">Contact</NuxtLink>
                        <NuxtLink to="/packages" class="link link-hover">Packages</NuxtLink>
                        <NuxtLink to="/lovina-dolphin-watching-tour" class="link link-hover">Lovina Dolphin Watching
                        </NuxtLink>
                        <NuxtLink to="/lovina-dolphin-and-snorkeling" class="link link-hover">Lovina Dolphin
                            Watching and Snorkeling</NuxtLink>
                        <NuxtLink to="/lovina-dolphin-and-swimming-with-dolphin" class="link link-hover">Lovina
                            Dolphin Watching and Swimming With Dolphin</NuxtLink>
                        <NuxtLink to="/sunset-plankton-tour" class="link link-hover">Sunset tour With Plankton
                        </NuxtLink>
                        <NuxtLink to="/fishing-tour-at-lovina" class="link link-hover">Fishing Tour at Lovina
                        </NuxtLink>
                        <NuxtLink to="/lovina-snorkeling-at-coral-reef" class="link link-hover">Snorkeling at lovina
                            coral reef</NuxtLink>
                    </li>





                </ul>
            </div>
            <NuxtLink to="/" class="btn btn-ghost normal-case text-gray-800 text-xl">Lovina Ocean Tours</NuxtLink>
        </div>
        <div class="navbar-end text-gray-800 hidden lg:flex">
            <ul class="menu menu-horizontal px-1 ">
                <NuxtLink to="/about" class="link btn btn-ghost  link-hover">About</NuxtLink>
                <NuxtLink to="/contact" class="link btn btn-ghost link-hover">Contact</NuxtLink>
                <NuxtLink to="/packages" class="link btn btn-ghost link-hover">Packages</NuxtLink>

            </ul>
        </div>

    </div>
</template>