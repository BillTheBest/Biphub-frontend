<style scoped lang="scss" src="./Card.scss"></style>

<template>
    <div class="card">
        <div v-bind:class="cardClass">
            <a v-bind:href="link">
                {{ title }}
            </a>
        </div>
        <div class="">
            {{ writer_name }}
        </div>
        <div class="">
            {{ crdate }}
        </div>
    </div>
</template>

<script>
    export default {
        props: {
            title: { type: String, default: 'N/A' },
            link: { type: String, default: 'http://google.com' },
            writer_name: { type: String, default: 'N/A' },
            writer_icon: { type: String, default: 'N/A' },
            crdate: { type: String, default: '1999-11-11' },
            bgColor: { type: String, default: 'gray' },
            computed: {

                // TODO: check why not work
                cardClass() {
                    console.log("####color:", this.bgColor);
                    switch (this.bgColor) {
                        case "gray":
                        case "default":
                            return "card-gray"
                            break
                    }
                }
            }
        }
    }
</script>
