<template>
<div>
    <div class="BoardMembersText">Board members</div>
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

<style scoped>

.BoardMembersText{
    text-decoration: green wavy underline;
    font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    text-align: center;
    font-size: 20px;
    font-weight: bold;
    padding-top: 20px;
}
</style>
