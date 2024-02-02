<template>
    
    <div class="intro">
        <div class="left">
            <h2>Ulrika Andersson</h2>
            <p>Hej! Jag är en personlig tränare med många års erfarenhet
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit voluptatum quis voluptate facere commodi? Eligendi vitae blanditiis eveniet delectus maxime exercitationem magnam accusamus harum nisi omnis? Iste autem nostrum modi eaque quasi incidunt illum non. Ipsa, incidunt odit? Quasi magnam quas accusantium nisi laboriosam ab nihil laudantium quam sed minus quaerat modi dolor quisquam totam sunt, incidunt explicabo ipsam molestiae nesciunt optio veniam quae!
            </p>
        </div>
        <div class="right">
            <img src="../assets/16af2ddf-6e33-4dcd-af20-6a1a802af6ca.webp" alt="">
        </div>
    </div>
    <Timeline />
</template>
<script>
import Timeline from '../components/TimeLine.vue';

export default {
    name: 'aboutme',
    components: {
        // Register the component
        Timeline
    }
    // component logic
}
</script>
<style>
.intro{
    margin-top: 3rem;
    display: flex;
    justify-content: space-around;
}
.left{
    padding:0rem 5rem;

}
.left p{
    font-size: 16px;
    margin-top: 1rem;
}
.right img{
    width:300px;
}
@media screen and (max-width:900px) {
    .intro{
        flex-direction: column;
        align-items: center;
        gap:2rem;
    }
    .left{
        padding:0rem 2rem;
    }
    
}
</style>