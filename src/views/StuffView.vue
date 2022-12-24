<template>
<div>
    <BoardMembers></BoardMembers>
    <BoardMembers></BoardMembers>
    <BoardMembers></BoardMembers>
    <BoardMembers></BoardMembers>
    <DeveloperTeam></DeveloperTeam>

</div>
</template>

<script>
import DeveloperTeam from "@/components/DeveloperTeam.vue"
import BoardMembers from "@/components/boardMeamber.vue"

export default {
    components: {
        DeveloperTeam:DeveloperTeam,
        BoardMembers:BoardMembers
    }
}
</script>
