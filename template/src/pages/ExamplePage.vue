<template>
    <v-container>
        <h3 class="my-3">Examples</h3>
        <h4>Cards</h4>
        <v-card>
            <v-card-media
                    src="https://images.unsplash.com/photo-1439886183900-e79ec0057170?dpr=1&auto=compress,format&fit=crop&w=991&h=608&q=80&cs=tinysrgb&crop="
                    height="300px">
                <v-container fill-height fluid>
                    <v-layout fill-height>
                        <v-flex xs12 align-end flexbox>
                            <span class="headline white--text">Card title</span>
                        </v-flex>
                    </v-layout>
                </v-container>
            </v-card-media>
            <v-card-text>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium amet at cupiditate dolorem doloribus esse expedita ipsum magnam necessitatibus neque, optio perferendis placeat porro quas quisquam repellat repellendus reprehenderit ut.
            </v-card-text>
            <v-card-actions class="blue-grey darken-1">
                <v-btn flat class="white--text">This is a button</v-btn>
                <v-spacer></v-spacer>
                <v-icon class="white--text">explore</v-icon>
            </v-card-actions>
        </v-card>
        <br>
        <h4>Dialogs</h4>

        <template>
            <v-layout row justify-center style="position: relative;">
                <v-dialog v-model="dialog" lazy absolute>
                    <v-btn primary dark slot="activator">Show dialog</v-btn>
                    <v-card>
                        <v-card-title>
                            <div class="headline">This is a simple dialog?</div>
                        </v-card-title>
                        <v-card-text>
                            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aliquid, deserunt ea eius nemo praesentium sint voluptates voluptatum. Enim modi natus, quaerat quibusdam sint voluptate. Consequatur enim excepturi provident repellat sequi?
                        </v-card-text>
                        <v-card-actions>
                            <v-spacer></v-spacer>
                            <v-btn class="green--text darken-1" flat="flat" @click.native="dialog = false">Sure</v-btn>
                            <v-btn class="green--text darken-1" flat="flat" @click.native="dialog = false">Maybe not
                            </v-btn>
                        </v-card-actions>
                    </v-card>
                </v-dialog>
            </v-layout>
        </template>
    </v-container>
</template>

<script>
  export default {
    data() {
      return {
        dialog: false,
      };
    },

    mounted() {
    },
  };
</script>
