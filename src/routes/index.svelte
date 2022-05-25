<script>
    import "$lib/index.css"
    let current1 = false;
    let current2 = false;
    let current3 = false;
    let current4 = false;
    let current5 = false;

    // /**
    // * @param {boolean} arg1
    // */
   
    // function handleClick(arg1){
    //     arg1 = !arg1;
    //     console.log("arg1: " + arg1);
    //     console.log("current1: " + current1);
    //     console.log("current2: " + current2);
    // }
</script>

<div class="app">
    <div class="card">
    
        <div class="leftSide">
            <div class="wrapper" id="wrapper">
                <img class="woman" alt="Woman" src="/illustration-woman-online-desktop.svg"/>
            </div>
            <img class="atSymbol" alt="at symbol" src="/illustration-box-desktop.svg"/>
        </div>

        <div class="rightSide">
            <h1>FAQ</h1>
            <!-- <img alt="The project logo" src={Arrow}/> -->
            
            <p class="{current1 === true ? 'questionSelected' : 'question'}"
                on:click={() => current1 = !current1}               
            >How many team members can I invite? </p>

            <p class="{current1 === true ? 'answerReveal' : 'answer'}">You can invite up to 5 team members. For additional members, upgrade to PRO.</p>
            <hr class="solid">

            <p class="{current2 === true ? 'questionSelected' : 'question'}"
                on:click="{ () => current2 = !current2}">What is the maximum file upload size?</p>
            <p class="{current2 === true ? 'answerReveal' : 'answer'}">No more than 2GB. All files in your account must fit your allotted storage space.</p>
            <hr class="solid">

            <p class="{current3 === true ? 'questionSelected' : 'question'}"
                on:click="{ () => current3 = !current3}">How do I reset my password?</p>
            <p class="{current3 === true ? 'answerReveal' : 'answer'}">Please visit your user settings to reset password.</p>
            <hr class="solid">

            <p class="{current4 === true ? 'questionSelected' : 'question'}"
                on:click="{ () => current4 = !current4}">Can I cancel my subscription?</p>
            <p class="{current4 === true ? 'answerReveal' : 'answer'}">You can end your subscription by selecting the End Membership button under user settings</p>
            <hr class="solid">

            <p class="{current5 === true ? 'questionSelected' : 'question'}"
                on:click="{ () => current5 = !current5}">Do you provide additional support?</p>
            <p class="{current5 === true ? 'answerReveal' : 'answer'}">Additional support and feedback can be found through our Slack page. </p>
            <hr class="solid">
        </div>
    </div>

    <footer>
        <p class="attribution">
          Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. 
          Coded by <a href="https://github.com/ssrivastava17">Stephanie Srivastava</a>.
        </p>
      </footer>
</div>