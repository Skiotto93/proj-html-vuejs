<script>
export default {
    name: 'ThirdSectionMain'
}
</script>

<template>
    <section>
        <div class="tab">
            <div class="titleTab">
                <h1>Upcoming Events</h1>
                <div class="events">
                    <div class="col-left">
                        <div class="calendar">
                            <span>07</span>
                            <div>Jan, 2022</div>
                        </div>
                    </div>
                    <div class="col-right">
                        <h3>Melbourne Coaching</h3>
                        <div class="d-flex">
                            <i class="fa-regular fa-clock"></i>
                            <p>9:00 am - 5:00 pm, Jan 7, 2022</p>
                        </div>
                        <div class="d-flex">
                            <i class="fa-solid fa-location-dot"></i>
                            <p>Cambridge, MA 02138, USA</p>
                        </div>
                        <h4>READ MORE</h4>
                    </div>
                </div>
                <div class="events">
                    <div class="col-left">
                        <div class="calendar">
                            <span>11</span>
                            <div>Jan, 2022</div>
                        </div>
                    </div>
                    <div class="col-right">
                        <h3>New York Coaching</h3>
                        <div class="d-flex">
                            <i class="fa-regular fa-clock"></i>
                            <p>9:00 am - 5:00 pm, Jan 11, 2022</p>
                        </div>
                        <div class="d-flex">
                            <i class="fa-solid fa-location-dot"></i>
                            <p>Cambridge, MA 02138, USA</p>
                        </div>
                        <h4>READ MORE</h4>
                    </div>
                </div>
                <div class="events">
                    <div class="col-left">
                        <div class="calendar">
                            <span>21</span>
                            <div>Jan, 2022</div>
                        </div>
                    </div>
                    <div class="col-right">
                        <h3>London Coaching</h3>
                        <div class="d-flex">
                            <i class="fa-regular fa-clock"></i>
                            <p>9:00 am - 5:00 pm, Jan 21, 2022</p>
                        </div>
                        <div class="d-flex">
                            <i class="fa-solid fa-location-dot"></i>
                            <p>Cambridge, MA 02138, USA</p>
                        </div>
                        <h4>READ MORE</h4>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
section {
    background-image: url('../img/h1-img-09.jpg');
    height: 1060px;
    background-position: center;
    background-size: cover;
    position: relative;
    .tab {
        width: 520px;
        width: 520px;
        position: absolute;
        top: 190px;
        left: 300px;
        .titleTab {
            background-color: #fafafa;
            h1 {
                border-bottom: 1px solid lightgrey;
                padding: 35px 40px;
            }
            .events:hover {
                background-color: #fff;
                background: linear-gradient(to bottom, #a6a6a6 0.2%, #fff 5px);
                h3 {
                        color: #ff4612;
                    }
            }
            .events {
                padding: 35px 40px;
                display: flex;
                border-bottom: 1px solid lightgrey;
                
                .col-left {
                    width: 25%;
                    .calendar {
                        background-color: #ff4612;
                        text-align: center;
                        padding: 15px;
                        span {
                            color: #fff;
                            padding-bottom: 10px;
                        }
                        div {
                            color: #ffb39e;
                        }
                    }
                }
                .col-right {
                    width: 75%;
                    padding: 0 25px;
                    h3 {
                        padding-bottom: 10px;
                    }
                    
                    .d-flex {
                        display: flex;
                        padding-bottom: 10px;
                        i {
                            margin-right: 10px;
                            color: #ff4612;
                        }
                        p {
                            color: #a6a6a6;
                        }
                    }
                }
            }
        }
    }
}
</style>