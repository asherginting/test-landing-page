<script>
    import {
        Carousel,
        CarouselControl,
        CarouselIndicators,
        CarouselItem,
        CarouselCaption,
    } from "sveltestrap";

    const items = [
        {
            url:
                "../img/bg.png",
            title: "Take your career to the next level 1",
            subTitle:
                "With indispensable courses 1",
        },
        {
            url:
                "../img/bg.png",
            title: "Take your career to the next level 2",
            subTitle:
                "With indispensable courses 2",
        },
        {
            url:
                "../img/bg.png",
            title: "Take your career to the next level 3",
            subTitle:
                "With indispensable course 3",
        },
    ];
    let activeIndex = 0;
</script>

<Carousel {items} bind:activeIndex ride={true} interval={2000}>
    <CarouselIndicators bind:activeIndex {items} />

    <div class="carousel-inner">
        {#each items as item, index}
            <CarouselItem bind:activeIndex itemIndex={index}>
                <img
                    src={item.url}
                    class="d-block w-100"
                    height="600"
                    alt={item.title}
                />
                <CarouselCaption
                    class="text-light"
                    captionHeader={item.title}
                    captionText={item.subTitle}
                />
            </CarouselItem>
        {/each}
    </div>

    <CarouselControl direction="prev" bind:activeIndex {items} />
    <CarouselControl direction="next" bind:activeIndex {items} />
</Carousel>
