<template>
    <div class="contact">
        <h1>This is an contact page</h1>

        <v-form v-model="valid">
            <v-container>
                <v-row>
                    <v-col cols="12" md="4">
                        <v-text-field
                            v-model="firstname"
                            :rules="nameRules"
                            :counter="10"
                            label="First name"
                            required
                        ></v-text-field>
                    </v-col>

                    <v-col cols="12" md="4">
                        <v-text-field
                            v-model="lastname"
                            :rules="nameRules"
                            :counter="10"
                            label="Last name"
                            required
                        ></v-text-field>
                    </v-col>

                    <v-col cols="12" md="4">
                        <v-text-field
                            v-model="email"
                            :rules="emailRules"
                            label="E-mail"
                            required
                        ></v-text-field>
                    </v-col>
                </v-row>

                <v-row>
                    <v-textarea
                        autocomplete="message"
                        label="Message"
                    ></v-textarea>
                </v-row>

                <v-row>
                    <v-btn block>
                        Submit!!
                    </v-btn>
                </v-row>
            </v-container>
        </v-form>

        <Footer />
    </div>
</template>

<script>
import Footer from '@/components/Footer';
export default {
    
    
    components: { Footer },
    data: () => ({
        valid: false,
        firstname: '',
        lastname: '',
        nameRules: [
            (v) => !!v || 'Name is required',
            (v) => v.length <= 10 || 'Name must be less than 10 characters',
        ],
        email: '',
        emailRules: [
            (v) => !!v || 'E-mail is required',
            (v) => /.+@.+/.test(v) || 'E-mail must be valid',
        ],
    }),
};
</script>
