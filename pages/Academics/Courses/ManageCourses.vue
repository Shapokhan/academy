<template>
<b-row class="CompleteRow">
    <b-col cols="3" class="LeftMenuCol">
        <leftmenu/> 
    </b-col>
    <b-col cols="9" class="contentarea">
        <h1>Manage Courses</h1>
    </b-col>
</b-row>
</template>

<script>
import leftmenu from '@/components/leftmenu'
export default {
    components:
    {
        leftmenu
    }

}
</script>

<style lang="scss">
@import "@/assets/_variables.scss";
.CompleteRow{
.contentarea
{
    background-color: $lightblack;
    padding: 0px;
    margin: 0px;
}
.LeftMenuCol{
    margin: 0px;
    padding: 0px;
}
}


</style>
