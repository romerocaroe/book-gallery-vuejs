<template>
    <div class="container">
        <div class="row">
            <div class="col-4" v-for="(book, index) in books" :key="index">
                <book :book="book" />
            </div>
        </div>
    </div>
</template>

<script>
    import Book from './Book.vue'

    export default {
        name: 'Gallery',
        components: { Book },
        data(){
            return {
                books: [
                    {
                        "title": "The Code of the Extraordinary Mind",
                        "author": "Vishen Lakhiani",
                        "img": "https://firebasestorage.googleapis.com/v0/b/fullstack-extraordinary.appspot.com/o/books%2Fthe-code-of-the-extraordinary-mind-3.png?alt=media&token=35295678-9534-4887-9310-eb0d722c052c"
                    },
                    {
                        "title": "Outliers",
                        "author": "Malcolm Gladwell",
                        "img": "https://firebasestorage.googleapis.com/v0/b/fullstack-extraordinary.appspot.com/o/books%2FOutliers.png?alt=media&token=a5c1d4c8-4117-42d1-b1fd-b4ea76ca4ce8"
                    },
                    {
                        "title": "Blink",
                        "author": "Malcolm Gladwell",
                        "img": "https://firebasestorage.googleapis.com/v0/b/fullstack-extraordinary.appspot.com/o/books%2Fblink.png?alt=media&token=cad9b311-878f-489b-ac26-018f57e665b2"
                    },
                    {
                        "title": "Limitless",
                        "author": "Jim Kwik",
                        "img": "https://firebasestorage.googleapis.com/v0/b/fullstack-extraordinary.appspot.com/o/books%2FLimitless.png?alt=media&token=2c643e4f-721f-4caa-b6b1-0e8c3e8ae4a7"
                    },
                    {
                        "title": "Flow",
                        "author": "Mihály Csikszentmihályi",
                        "img": "https://firebasestorage.googleapis.com/v0/b/fullstack-extraordinary.appspot.com/o/books%2Fflow.png?alt=media&token=b9ed45d9-bce4-4ce5-9cf1-12fc15470f6d"
                    }
                ]
            }
        }
    }
</script>

<style scoped>

</style>