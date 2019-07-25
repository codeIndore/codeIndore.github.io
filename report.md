---
layout: default
permalink: /report/
title: Report
---
<h1 class="has-text-centered">{{ page.title }}</h1>
<p class="has-text-centered">Please use this form to report any violations of the <a href="/coc/" target="_blank">Code of Conduct</a>. <br />Reports can be submitted anonymously. Please include all relevant details in your response. <br />The responses will be kept confidential.</p>
<br />
<form action="https://docs.google.com/forms/d/e/1FAIpQLScmT7k9J209Fd0729n6iiDzy34A8Hx_dreIicC7_HWOCoSmYg/formResponse"
      target="_self"
      id="bootstrapForm"
      method="POST">

    <!-- Field type: "short" id: "826355120" -->
    <div class="field is-horizontal">
    <div class="field-label">
        <legend class="label" for="826355120">Name</legend>
        </div>
        <div class="field-body">
            <input id="2092238618" type="text" name="entry.2092238618" class="input" placeholder="Name">
        </div>
    </div>


    <!-- Field type: "short" id: "2071572813" -->
    <div class="field is-horizontal">
    <div class="field-label">
        <legend class="label" for="2071572813">Email</legend>
        </div>
        <div class="field-body">
            <input id="297764783" type="text" name="entry.297764783" class="input" placeholder="email@domain.tld">
        </div>
    </div>


    <!-- Field type: "short" id: "569514487" -->
    <div class="field is-horizontal">
    <div class="field-label">
        <legend class="label" for="569514487">Phone Number</legend>
        </div>
        <div class="field-body">
            <input id="1966605262" type="text" name="entry.1966605262" class="input" placeholder="+91 99999 12345">
        </div>
    </div>


    <!-- Field type: "short" id: "1517600930" -->
    <div class="field is-horizontal">
    <div class="field-label">
        <legend class="label" for="1517600930">Violator details</legend>
        </div>
        <div class="field-body">
            <input id="1340835164" type="text" name="entry.1340835164" class="input" placeholder="Violator's name or other description">
        </div>
    </div>


    <!-- Field type: "short" id: "245385898" -->
    <div class="field is-horizontal">
    <div class="field-label">
        <legend class="label" for="245385898">Date of incident</legend>
    </div>
        <div class="field-body">
            <input id="479301265" type="text" name="entry.479301265" class="input" placeholder="DD/MM/YYYY" required>
        </div>
    </div>


    <!-- Field type: "short" id: "1312689492" -->
    <div class="field is-horizontal">
    <div class="field-label">
        <legend class="label" for="1312689492">Incident Details</legend>
        </div>
        <div class="field-body">
            <textarea id="1857009907" type="text" name="entry.1857009907" class="textarea" placeholder="Please include all details of the incident." required></textarea>
        </div>
    </div>

    <input type="hidden" name="fvv" value="1">
    <input type="hidden" name="fbzx" value="4765250700995431190">
    <input type="hidden" name="pageHistory" value="0">
    <br />
    <div class="has-text-centered">
        <input class="button is-link" type="submit" value="Submit">
    </div>
</form>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.2.1/jquery.min.js" integrity="sha256-hwg4gsxgFZhOsEEamdOYGBf13FyQuiTwlAQgxVSNgt4=" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery.form/4.2.2/jquery.form.min.js" integrity="sha256-2Pjr1OlpZMY6qesJM68t2v39t+lMLvxwpa8QlRjJroA=" crossorigin="anonymous"></script>
<script type="text/javascript">
$('#bootstrapForm').submit(function (event) {
    event.preventDefault()
    var extraData = {}
    $('#bootstrapForm').ajaxSubmit({
        data: extraData,
        dataType: 'jsonp',  // This won't really work. It's just to use a GET instead of a POST to allow cookies from different domain.
        error: function () {
            alert('Report Received. Appropriate actions will be taken as defined in the Code of Conduct.')
        }
    })
})
</script>
