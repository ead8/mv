<script lang="ts">
    import { Play } from 'lucide-svelte';
    let videoElement: HTMLVideoElement;
    let isPlaying = false;

    function togglePlay() {
        if (videoElement.paused) {
            videoElement.play();
        } else {
            videoElement.pause();
        }
    }

    // Handle clicks directly on the video
    function handleVideoClick() {
        togglePlay();
    }
</script>

<section class="bg-[#F5EFE6] py-20">
    <div class="mx-auto max-w-6xl px-4">
        <div class="mx-auto mb-12 max-w-3xl text-center">
            <h2 class="mb-6 font-serif text-4xl text-[#5C4937] lg:text-5xl">Our Work in Action</h2>
            <p class="leading-relaxed text-[#766D66]">
                Experience our design journey through a showcase of projects that blend creativity,
                functionality, and innovation. Watch the video to see how we bring spaces to life.
            </p>
        </div>

        <div class="group relative overflow-hidden rounded-2xl">
            <video
                bind:this={videoElement}
                src="/videos/classical (1).mp4"
                poster="/images/overlay.png"
                class="h-auto w-full rounded-2xl object-cover cursor-pointer"
                preload="auto"
                on:play={() => isPlaying = true}
                on:pause={() => isPlaying = false}
                on:click={handleVideoClick}
            >
                <source src="/videos/classical (1).mp4" type="video/mp4">
            </video>

            {#if !isPlaying}
            <div class="absolute inset-0 flex items-center justify-center bg-black/20 transition-colors duration-300 group-hover:bg-black/30">
                <button
                    on:click={togglePlay}
                    class="flex h-16 w-16 transform items-center justify-center rounded-full bg-white shadow-lg transition-transform duration-300 group-hover:scale-110"
                    aria-label="Play video"
                >
                    <Play class="ml-1 h-8 w-8 text-[#5C4937]" />
                </button>
            </div>
            {/if}
        </div>
    </div>
</section>