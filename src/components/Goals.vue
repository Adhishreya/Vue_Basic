<template>
  <div class="container">
    <div class="row">
      <h4 class="col-12 describe-3">Set ur contribution goals right away!!!</h4>
      <div class="row">
        <div class="col-12 col-lg-6">
          <ul class="list-group">
            <Template
              v-for="(i, index) in goals"
              :data="i.goal"
              :complete="i.check"
              :key="index"
            />
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import Template from "./Template";
export default {
  name: "Goals",
  components: {
    Template,
  },
  data() {
    return {
      // hardcoding the data which later will be integreated with thre user iput
      goals: [
        { goal: "Create a github account", check: true },
        { goal: "Learn git basics", check: true },
        { goal: "Create first PR", check: false },
        { goal: "Solve an issue", check: true },
      ],
    };
  },
  //creating the facility for the user to manipulate the data
  user_edit: {
    add_goal(req_goal) {
      //add the goals set by the user in the goals list
      this.goals.push({ goal: req_goal, check: false });
    },
    //allows the user to toggle between checked and unchecked
    toggle_goal(req_goal) {
      req_goal.ckeck = !req_goal.check;
    },
    edit(req_goal, new_goal) {
      req_goal.goal = new_goal.goal;
    },
    delete_goal(d_goal) {
      this.goals = this.goals.filter(
        (ret_goal) => ret_goal.goal !== d_goal.goal
      );
    },
  },
};
</script>
<style scoped>
</style>