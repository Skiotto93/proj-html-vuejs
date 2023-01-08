<script>
export default {
    name: 'AppHeaderSon',
    props: {
        title: String,
        text: String,
        image: String,
        index: Number,
    }
}
</script>

<template>
    <div class="text-header">       
        <h1>{{ title }}<span class="oragePoint">.</span></h1>
        <p>
            {{ text }}
        </p>
        <div class="headerBtn">
            <button type="button" class="button-white">
                READ MORE
                <div>
                    <i class="fa-solid fa-arrow-right-long"></i>
                </div>
            </button>
            <button type="button" class="button-orange">
                PURCHASE
                <div>
                    <i class="fa-solid fa-arrow-right-long"></i>
                </div>
            </button>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .inactive {
        display: none;
    }
    .text-header {
        max-width: 600px;
        position: absolute;
        bottom: 35%;
        right: 55%;
        
        h1 {
            font-size: 70px;
            padding: 20px 0;
            span {
                color: #ff4c19;
            }
        }
        p {
            padding-bottom: 20px;
        }
        .headerBtn {
            padding: 20px 0;
            display: flex;
            
            .button-white {
                padding: 10px;
                background-color: white;
                display: flex;
                border: none;
                cursor: pointer;
                div {
                    margin-left: 20px;
                    padding-left: 10px;
                    border-left: 1px solid;
                    i {
                        width: 30px;                        
                    }
                }
                div:hover {
                    border-left: none;
                }
            }
            .button-orange {
                padding: 10px;
                margin-left: 20px;
                background-color: #ff4c19;
                color: #fff;
                display: flex;
                border: none;
                cursor: pointer;
                div {
                    margin-left: 20px;
                    padding-left: 10px;
                    border-left: 1px solid;
                }
                div:hover {
                    border-left: inherit;
                }
            }
        }
    }
</style>