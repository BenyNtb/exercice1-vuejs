<template>
    <div>
        <!-- <h1>Shift the overall look and feel by adding these wonderful touches to furniture in your home</h1> -->
        <h1>{{ titre }}</h1>
        <p id="para1"> {{para1}}</p>
        <p id="nom">{{nom}}</p>
        <p id="date">{{date}}</p>
        <ul v-show="!isNinja">
            <!-- <li><img alt="facebook">{{fb}}</li>
            <li><img alt="twitter">{{twitter}}</li>
            <li><img alt="pinterest">{{pinterest}}</li> -->
        </ul>
    </div>
</template>


<script>

    export default {
        name: 'Test',
        props: {
            msg: String,
            para1: String,
            titre: String,
            nom:String,
            date: Date,
            fb:String,
            twitter:String,
            pinterest: String,
            img:String,
        },
    }

</script>

