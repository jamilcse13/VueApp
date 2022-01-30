## List Rendering:
- v-for (for loop)
    - v-for="n in 5"
    - v-for="framework in topTenFrameworks"
    - v-for="(framework, index) of topTenFrameworks"
    - v-for="(score, framework) of topTenFrameworks"

## Event Rendering:
- v-on:click Or @click
    - v-on:click="upvote(framework)"    //call a function
- v-on:mousemove
    - v-on:mousemove="getCoordinates"   //call a function
- v-on:submit.prevent
    - v-on:submit.prevent="handleSubmit"    //call a function
- v-on:model
    - v-model="framework"
- v-on:keyup
    - v-on:keyup.enter="handleSubmit"   //call a function
    - v-on:keyup.esc="clearText"    //call a function

## Conditional Rendering:
- v-if : if true then each time render the whole conditional portion
- v-else
- v-else-if
    - v-if="!records.length"
    - v-else-if="records.length === 1"
- v-show : it doesn't render the portion each time, it just uses style: display or display none
    - v-show="showAlertSecondary"

## Class Binding:
- :class
    - :class="[hovered ? 'bg-primary' : 'bg-info']" 
        @mouseover="hovered = true" @mouseout="hovered = false"
    - :class="alertType"    //call a function

## Style Binding:
- :style
    - :style="myClasses"    //Object
    - :style="[style1, style2]"
    - :style="{ 'width': width + '%' }"

## Computed Properties
- when we write a logic inside computed, then we should return *fullName*
- when we write a logic inside methods, then we should return *fullName()*
- sort():
    - this.topTenFrameworks.sort((a, b) => (a.score - b.score) * this.order)


## Project DataVue
- 