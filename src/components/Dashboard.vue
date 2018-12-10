<template>
    <div class="hello">
        <nav class="navbar navbar-default navbar-fixed-top">
            <p class="navbar-text">Title...</p>
        </nav>

        <div class="btn btn-success m-5 display-4">
            Button
        </div>

        <div class="container-fluid">
            <div class="row">
                <!-- Nav left -->
                <ul class="nav col-md-2" id="leftTabs">
                    <li class="active">
                        <a href="#a_tab" data-toggle="tab">
                            <span></span>ItemA
                        </a>
                    </li>
                    <li>
                        <a href="#b_tab" data-toggle="tab">
                            <span></span>ItemB
                        </a>
                    </li>
                    <li>
                        <a href="#c_tab" data-toggle="tab">
                            <span></span>ItemC - TABS!
                        </a>
                    </li>
                </ul>
                <!-- Nav content -->
                <div class="tab-content col-md-10">
                    <div class="tab-pane active" id="a_tab">
                        <h1>Content of A</h1>
                    </div>
                    <div class="tab-pane" id="b_tab">
                        <h1>Content of B</h1>
                    </div>
                    <div class="tab-pane" id="c_tab">
                        <!-- Nav tabs -->
                        <ul class="nav nav-tabs">
                            <li class="active"><a href="#first" data-toggle="tab">First</a></li>
                            <li><a href="#second" data-toggle="tab">Second</a></li>
                            <li><a href="#third" data-toggle="tab">Third</a></li>
                        </ul>
                        <!-- Nav tabs content -->
                        <div class="tab-content">
                            <div id="first" class="tab-pane active">Content of first</div>
                            <div id="second" class="tab-pane">Content of second</div>
                            <div id="third" class="tab-pane">Content of third</div>
                        </div>

                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script lang="ts">
    import {
        Component,
        Prop,
        Vue
    } from 'vue-property-decorator';

    @Component
    export default class Dashboard extends Vue {
        @Prop() private msg!: string;
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    h3 {
        margin: 40px 0 0;
    }

    ul {
        list-style-type: none;
        padding: 0;
    }

    li {
        display: inline-block;
        margin: 0 10px;
    }

    a {
        color: #42b983;
    }

    body {
    padding-top: 60px;
    }
    .navbar {
    background-color: grey;
    min-height: 60px;
    }
    .navbar-default .navbar-text {
    color: #ffffff;
    }

    .tabbable {
    margin-top: 60px;
    }

    .tabs-left > .nav-tabs {
    border-bottom: 0;
    }
    .tab-content > .tab-pane {
    display: none;
    }
    .tab-content > .active {
    display: block;
    }
    .tabs-left > .nav-tabs > li {
    float: none;
    border-right: 1px solid #D3D3D3;
    margin-bottom: 1px;
    }
    .tabs-left > .nav-tabs > li > a {
    margin-right: 0;
    text-align: center;
    padding: 15px 15px;
    }
    .tabs-left > .nav-tabs {
    float: left;
    margin-right: 19px;  
    }
    .tabs-left > .nav-tabs .active > a,
    .tabs-left > .nav-tabs .active > a:hover,
    .tabs-left > .nav-tabs .active > a:focus {
    background-color: #d9d9d9;
    }

</style>