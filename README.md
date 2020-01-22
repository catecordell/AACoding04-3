
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width">
<meta name="csrf-param" content="authenticity_token" />
<meta name="csrf-token" content="KVAL7MNIeBTM9oGITA8L5lSwecl+g4kdehxRJj7p3mPDUMkjVpgxFx8BgpUqNKWX4v6liEqztjroUR86AGteLQ==" />
<title>AACoding04-2</title>
<link href='https://fonts.googleapis.com/css?family=Lato:300,400,400italic,700,700italic,900,900italic' rel='stylesheet'>
<meta name="description" content="...">
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:site" content="@CodePen">
<meta name="twitter:title" content="AACoding04-2">
<meta name="twitter:description" content="...">
<meta name="twitter:image" content="https://screenshot.codepen.io/3974065.mdyzOwZ.b3cda4ed-6a3b-4f69-b77c-6a9570610f07.png">
<meta property="og:image" content="https://codepen.io/catecordell/pen/mdyzOwZ/image/large.png" itemprop="thumbnailUrl">
<meta property="og:title" content="AACoding04-2">
<meta property="og:url" content="https://codepen.io/catecordell/details/mdyzOwZ">
<meta property="og:site_name" content="CodePen">
<meta property="og:description" content="...">
<meta name="apple-mobile-web-app-title" content="CodePen">
<script async src="https://www.googletagmanager.com/gtag/js?id=UA-30102653-2"></script>
<script>/* Firefox needs this to prevent FOUC */</script>
</head>
<body class="details logged-in sidebar-false not-team">
<div id="react-page"></div>
<div id="react-popups" class="react-popups"></div>
<noscript>

  <input type="checkbox" class="modal-closing-trick" id="modal-closing-trick">

  <div class="overlay noscript-overlay" style="display: block;"></div>

  <div class="modal modal-message group modal-warning">

    <div class="modal-title">CodePen doesn't work very well without JavaScript.</div>

    <p>We're all for progressive enhancement, but CodePen is a bit unique in that it's all about writing and showing front end code, including JavaScript. It's required to use most of the features of CodePen.</p>

    <p>Need to know how to enable it? <a href="http://enable-javascript.com/" target="_blank" rel="noopener">Go here.</a></p>

    <label class="button button-medium" for="modal-closing-trick">Close this, use anyway.</label>

  </div>

</noscript>
<input type="hidden" id="init-data" value="{&quot;__browser&quot;:{&quot;device&quot;:&quot;unknown&quot;,&quot;mobile&quot;:null,&quot;name&quot;:&quot;chrome&quot;,&quot;platform&quot;:&quot;pc&quot;,&quot;version&quot;:&quot;79&quot;},&quot;__analytics&quot;:{&quot;controllerActionName&quot;:&quot;show&quot;,&quot;controllerName&quot;:&quot;details&quot;,&quot;enabled&quot;:true},&quot;__remote_addr&quot;:&quot;73.225.116.10&quot;,&quot;__CPDATA&quot;:{&quot;domain_iframe&quot;:&quot;https://cdpn.io&quot;,&quot;host&quot;:&quot;codepen.io&quot;,&quot;iframe_allow&quot;:&quot;geolocation; microphone; camera; midi; vr; accelerometer; gyroscope; payment; ambient-light-sensor; encrypted-media&quot;,&quot;iframe_sandbox&quot;:&quot;allow-forms allow-modals allow-pointer-lock allow-popups allow-presentation allow-same-origin allow-scripts&quot;},&quot;__env&quot;:&quot;production&quot;,&quot;__turnOffJS&quot;:false,&quot;__constants&quot;:{&quot;grid_iframe_sandbox_attributes&quot;:&quot;allow-scripts allow-pointer-lock allow-same-origin&quot;},&quot;__svg_sprite&quot;:&quot;/svg_sprite?v=8885a907&quot;,&quot;__user&quot;:{&quot;anon&quot;:false,&quot;base_url&quot;:&quot;/catecordell/&quot;,&quot;current_team_id&quot;:0,&quot;current_team_hashid&quot;:&quot;YdEzGn&quot;,&quot;hashid&quot;:&quot;yYzKVJ&quot;,&quot;id&quot;:3974065,&quot;itemType&quot;:&quot;user&quot;,&quot;name&quot;:&quot;Cate Cordell&quot;,&quot;owner_id&quot;:&quot;yYzKVJYdEzGn&quot;,&quot;paid&quot;:false,&quot;tier&quot;:0,&quot;username&quot;:&quot;catecordell&quot;},&quot;__firestore&quot;:{&quot;config&quot;:{&quot;apiKey&quot;:&quot;AIzaSyBgLAe7N_MdFpuVofMkcQLGwwhUu5tuxls&quot;,&quot;authDomain&quot;:&quot;codepen-store-production.firebaseapp.com&quot;,&quot;databaseURL&quot;:&quot;https://codepen-store-production.firebaseio.com&quot;,&quot;disabled&quot;:false,&quot;projectId&quot;:&quot;codepen-store-production&quot;},&quot;token&quot;:&quot;eyJhbGciOiJSUzI1NiJ9.eyJhdWQiOiJodHRwczovL2lkZW50aXR5dG9vbGtpdC5nb29nbGVhcGlzLmNvbS9nb29nbGUuaWRlbnRpdHkuaWRlbnRpdHl0b29sa2l0LnYxLklkZW50aXR5VG9vbGtpdCIsImNsYWltcyI6eyJvd25lcklkIjoieVl6S1ZKWWRFekduIiwiYWRtaW4iOmZhbHNlfSwiZXhwIjoxNTc5NjY4Nzg2LCJpYXQiOjE1Nzk2NjUxODYsImlzcyI6ImZpcmViYXNlLWFkbWluc2RrLThva3lsQGNvZGVwZW4tc3RvcmUtcHJvZHVjdGlvbi5pYW0uZ3NlcnZpY2VhY2NvdW50LmNvbSIsInN1YiI6ImZpcmViYXNlLWFkbWluc2RrLThva3lsQGNvZGVwZW4tc3RvcmUtcHJvZHVjdGlvbi5pYW0uZ3NlcnZpY2VhY2NvdW50LmNvbSIsInVpZCI6InlZektWSiJ9.szH8an2re8efIFO1uS_luqCP35ujrqA-TOXxRqIpSJfx2MTgkzUJcbQMWLfIHkQUw8QGAVQ-ROh5FnPta504SRB4lI9LD9VokgIdq6IEPSxq1WraHfUNAfaw_JB6jaM1kEFxeruI5AYMv7Z3_0YgbcEkaeY0kjV8aLFm5sfVMfjn_rnXFoLF9-DyMDHqI1QfRcw0eXj4OGHgvK-R5MtcOVf_3SrcK6YCAAAVkeDXNty79XFLP-ka9tytcfKWZCeM1pRHZHFYVklUBiLvHm5smHQ3-3ri6RMTQFh5atXIuDof7T90qKL_5LS3oPUMRMQVIzFJW6IOWuezcMjmYPPfVA&quot;},&quot;__graphql&quot;:{&quot;data&quot;:{&quot;sessionUser&quot;:{&quot;id&quot;:&quot;yYzKVJ&quot;,&quot;name&quot;:&quot;Cate Cordell&quot;,&quot;avatar80&quot;:&quot;https://gravatar.com/avatar/15e29d5769b2e4d5c6f976e2693fe7a5?s=80&amp;d=https://static.codepen.io/assets/avatars/user-avatar-80x80-bdcd44a3bfb9a5fd01eb8b86f9e033fa1a9897c3a15b33adfc2649a002dab1b6.png&quot;,&quot;avatar512&quot;:&quot;https://gravatar.com/avatar/15e29d5769b2e4d5c6f976e2693fe7a5?s=512&amp;d=https://static.codepen.io/assets/avatars/user-avatar-512x512-6e240cf350d2f1cc07c2bed234c3a3bb5f1b237023c204c782622e80d6b212ba.png&quot;,&quot;canCreatePosts&quot;:false,&quot;currentContext&quot;:{&quot;id&quot;:&quot;yYzKVJ&quot;,&quot;baseUrl&quot;:&quot;/catecordell&quot;,&quot;title&quot;:&quot;Cate Cordell&quot;,&quot;name&quot;:&quot;Cate Cordell&quot;,&quot;avatar80&quot;:&quot;https://gravatar.com/avatar/15e29d5769b2e4d5c6f976e2693fe7a5?s=80&amp;d=https://static.codepen.io/assets/avatars/user-avatar-80x80-bdcd44a3bfb9a5fd01eb8b86f9e033fa1a9897c3a15b33adfc2649a002dab1b6.png&quot;,&quot;avatar512&quot;:&quot;https://gravatar.com/avatar/15e29d5769b2e4d5c6f976e2693fe7a5?s=512&amp;d=https://static.codepen.io/assets/avatars/user-avatar-512x512-6e240cf350d2f1cc07c2bed234c3a3bb5f1b237023c204c782622e80d6b212ba.png&quot;,&quot;username&quot;:&quot;catecordell&quot;,&quot;contextType&quot;:&quot;USER&quot;,&quot;projectLimitations&quot;:{&quot;projects&quot;:1,&quot;usedProjects&quot;:0,&quot;__typename&quot;:&quot;ProjectLimitations&quot;},&quot;privateByDefault&quot;:false,&quot;__typename&quot;:&quot;User&quot;},&quot;currentTeamId&quot;:null,&quot;baseUrl&quot;:&quot;/catecordell&quot;,&quot;username&quot;:&quot;catecordell&quot;,&quot;admin&quot;:false,&quot;anon&quot;:false,&quot;pro&quot;:false,&quot;verified&quot;:false,&quot;teams&quot;:[],&quot;permissions&quot;:{&quot;canCreatePrivate&quot;:false,&quot;__typename&quot;:&quot;UserPermissions&quot;},&quot;__typename&quot;:&quot;User&quot;}}}}">
<script src="https://static.codepen.io/assets/common/browser_support-1963aa6406ae47d3176af996336c5d219acd8913c5af309e72f18933e95201cc.js"></script>
<script src="https://static.codepen.io/assets/packs/js/vendor-81829010d958be8a91ac.chunk.js"></script>
<script src="https://static.codepen.io/assets/packs/js/3-a1c3d05659a47b0e7e4a.chunk.js"></script>
<script src="https://static.codepen.io/assets/packs/js/everypage-776a100c092437137e00.js"></script>
</body>
</html>
