<template>
  <div>
    <task-dialog-list></task-dialog-list>
    <ticket-item></ticket-item>
  </div>
</template>

<script>
  import TicketItem from '../components/LandingPage/TicketItem'
  import TaskDialogList from '../components/LandingPage/TaskDialogList'

  export default {
    name: 'landing-page',
    components: { TicketItem, TaskDialogList },
    methods: {
      open (link) {
        this.$electron.shell.openExternal(link)
      }
    }
  }
</script>

<style :scoped>
  @import url('https://fonts.googleapis.com/css?family=Source+Sans+Pro');

</style>
