<template>
    <div class="home">
        <v-container>
            <img
                alt="Logo"
                src="https://image.freepik.com/free-vector/web-development-programmer-engineering-coding-website-augmented-reality-interface-screens-developer-project-engineer-programming-software-application-design-cartoon-illustration_107791-3863.jpg"
            />

            <h1> Hello World from Front End Cafe</h1>

            <h2>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius
                deserunt, modi ab velit delectus impedit. Tenetur cum libero
                natus. Nostrum nobis quisquam
            </h2>

            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Expedita cumque aperiam maxime aliquam, amet animi molestias
                laboriosam rerum corporis, minima laudantium autem temporibus
                sint harum consequatur tempore. Aut, recusandae laboriosam.
            </p>

            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Expedita cumque aperiam maxime aliquam, amet animi molestias
                laboriosam rerum corporis, minima laudantium autem temporibus
                sint harum consequatur tempore. Aut, recusandae laboriosam.
            </p>

            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Expedita cumque aperiam maxime aliquam, amet animi molestias
                laboriosam rerum corporis, minima laudantium autem temporibus
                sint harum consequatur tempore. Aut, recusandae laboriosam.
            </p>
        </v-container>

        <Footer />
    </div>
</template>

<script>
// @ is an alias to /src
import Footer from '@/components/Footer';

export default {
    name: 'Home',
    components: { Footer }
};
</script>
