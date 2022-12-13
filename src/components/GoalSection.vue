<template>
  <div id="goal" class="offset">
    <div class="col-md-12 narrow text-center">
      <div class="message">
        &#8226; What is the difference between working remotely and freelancing?
      </div>
      <div class="message">
        &#8226; How to pass TopTal interview process and join the top 3% of Software
        Developers?
      </div>
      <div class="message">&#8226; How to start working remotely?</div>
      <div class="message">
        &#8226; How to find the best short-term and long-term projects?
      </div>
    </div>
    <div class="jumbotron">
      <div class="narrow text-center">
        <div class="row text-center">
          <div class="col-md-4">
            <Card title="Learn about working remotely" image="step1.png">
              <p>Get a full overview of Toptal advantages and learn how to start.</p>
            </Card>
          </div>
          <div class="col-md-4">
            <Card title="Prepare for the interview" image="step2.png">
              <p>
                Join our guided interview process to easily pass all interview steps and
                join top 3%
              </p>
            </Card>
          </div>
          <div class="col-md-4">
            <Card title="Start working on Toptal" image="step3.png">
              <p>
                Get the most interesting projects from all over the world. And learn how
                to find the best one.
              </p>
            </Card>
          </div>
        </div>
      </div>
    </div>
    <!-- </div> -->
  </div>
</template>

<script>
import Card from "./common/Card.vue";

export default {
  name: "GoalSection",
  components: {
    Card,
  },
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
#features .narrow {
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
</style>
