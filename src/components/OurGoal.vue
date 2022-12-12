<template>
        <div id="our goal" class="offset">
            <div class="col-md-12 narrow text-center">
                <div class="message">&#8226; What is the difference between working remotely and freelancing?</div>
                <div class="message">&#8226; How to pass TopTal interview process and join the top 3% of Software Developers?</div>
                <div class="message">&#8226; How to start working remotely?</div>
                <div class="message">&#8226; How to find the best short-term and long-term projects?</div>
            </div>
            <div class="jumbotron">
                <div class="narrow text-center">
                    <div class="row text-center">
                        <div class="col-md-4">
                            <div class="feature">
                                <img src="@/assets/images/step1.png" alt="">
                                <div class="description">
                                    <h3>Learn about working remotely</h3>
                                    <p>Get a full overview of Toptal advantages and learn how to start.</p>
                                </div>
                            </div>
                        </div>
                        <div class="col-md-4">
                            <div class="feature">
                                <img src="@/assets/images/step2.png" alt="">
                                <div class="description">
                                    <h3>Prepare for the interview</h3>
                                    <p>Join our guided interview process to easily pass all interview steps and join top 3%</p>
                                </div>
                            </div>
                        </div>
                        <div class="col-md-4">
                            <div class="feature">
                                <img src="@/assets/images/step3.png" alt="">
                                <div class="description">
                                    <h3>Start working on Toptal</h3>
                                    <p>Get the most interesting projects from all over the world. And learn how to find the best one.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        <!-- </div> -->
    </div>
</template>

<script>
export default {
    name: "our goal"
};
</script>

<style scoped>
.description {
    margin: 25px 0;
}
.message {
    font-size: 1.2rem;
    color: white;
}
.jumbotron {
    background-color: #101010;
    color: white;
}
img {
    width: 100%;
}
#features .narrow{
    padding-top: 0;
    background-color: #101010;
}
#features:before {
    background-color: #101010;
    display: block;
    content: "";
    height: 3.7rem;
    margin-top: -3.7rem;
}
.feature h3 {
    font-size: 1.3rem;
    text-transform: uppercase;
    padding-bottom: 0.4rem;
}
.feature p {
    font-size: 1.1rem;
}
</style>
