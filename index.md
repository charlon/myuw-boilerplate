---
layout: default
title: MyUW
permalink: /
---

{% assign user = site.data.profiles.[site.uw_logged_in] %}

{% if user.uw_notices %}
<div class="myuw-card">
    <h2>Notices</h2>
    <ul>
        <li>asldkjf</li>
        <li>asldjflk</li>
        <li>oasdjf</li>
    </ul>
</div>
{% endif %}

{% if user.uw_courses %}
<div class="myuw-card">
    <h2>Course Schedule</h2>
    <ul>
        {% for item in user.uw_courses %}
        <li>{{ item.name }}</li>
        {% endfor %}
    </ul>
</div>
{% endif %}

<div class="myuw-card">
    <h2>Card Content</h2>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus semper velit quis arcu pharetra vehicula. Donec id accumsan libero. Duis in tempus diam, id faucibus dui. Aenean molestie elit elementum, dictum massa nec, ornare lectus. Curabitur finibus, augue ac finibus pulvinar, ligula nisi commodo felis, fringilla pharetra dolor felis nec risus. Vivamus rutrum imperdiet lectus et feugiat. Vivamus dui lorem, malesuada eget elementum id, pulvinar nec turpis. Ut gravida, augue semper tincidunt efficitur, leo velit aliquet ligula, ac semper est tellus at elit. Etiam in massa tempor, blandit ipsum id, malesuada lorem. Proin arcu nulla, molestie semper eros dignissim, ornare porttitor mauris. Nam vel ligula at mi interdum eleifend. Aliquam eu vehicula purus.

    Suspendisse potenti. Curabitur finibus, purus tincidunt tincidunt rhoncus, mauris risus vehicula felis, consectetur bibendum augue odio vel nisi. Nullam ultrices vitae erat sollicitudin hendrerit. Vivamus imperdiet tortor at sollicitudin tristique. Donec elementum vulputate efficitur. Nullam elementum nunc efficitur dictum tincidunt. Donec commodo eros vel sapien facilisis tempor. Suspendisse gravida velit eu augue scelerisque, sit amet lobortis nisl scelerisque.

    Donec ut justo quis sem mollis suscipit. Ut vel mollis lorem. Curabitur quis orci sagittis, maximus justo at, congue libero. Morbi aliquam mauris et nisl euismod, eget elementum ex vulputate. Donec mi ex, commodo at arcu non, condimentum efficitur velit. Curabitur orci sapien, finibus ut leo sit amet, gravida rutrum metus. Donec nec nunc quis elit sodales placerat. Pellentesque eu rutrum magna. Nullam elementum nisi at imperdiet accumsan. Nunc accumsan ullamcorper massa eu tristique. Fusce pharetra sapien vel pretium pellentesque. Etiam rhoncus finibus libero.

    In hac habitasse platea dictumst. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras bibendum neque luctus facilisis molestie. Proin a facilisis lectus. Sed suscipit ipsum felis, vitae sollicitudin arcu dictum a. Morbi blandit venenatis tortor, id mollis diam tempus quis. Maecenas sit amet mauris erat. Nam tincidunt quam et nibh posuere mollis. Nullam et molestie augue, id tristique dolor. Nunc et pretium ipsum. Donec rhoncus tortor vel sapien rutrum, eget consectetur ex sodales. Sed aliquet consequat tellus, nec auctor metus condimentum non. Etiam tincidunt eros luctus nisl sagittis pulvinar. Quisque ultrices, velit et interdum dignissim, lacus dolor egestas neque, sed pretium ex massa ut est.
</div>
