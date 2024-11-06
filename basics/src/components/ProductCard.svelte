<script>
    export let productFeature
</script>

<div class="grid grid-cols-1 md:grid-cols-2 gap-10 md:gap-14 lg:gap-20 relative text-base">
    <div class="flex flex-col gap-8 md:gap-10">
        <h4 class="text-2xl sm:text-3xl md:text-4xl max-w-[1000px] w-full font-medium pr-10 relative after:absolute after:top-full after:left-0 after:w-1/5 after:h-1.5 after:mt-1 after:bg-slate-100">
            <slot />
        </h4>
        <p>{productFeature.description}</p>
        <div class="flex flex-col gap-3">
            {#each productFeature.featureList as listItem}
                <div class="flex gap-2 items-center">
                    <div class="grid place-items-center px-1.5 text-xs sm:text-sm aspect-square rounded-full border-[1.5] bg-white border-solid border-green-300">
                        <i class="fa-solid fa-bolt text-green-400"></i>
                    </div>
                    <p>{listItem}</p>
                </div>
            {/each}
        </div>
    </div>
</div>
