<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Live Link Button</title>
  <style>
    :root{
      --btn-bg: #0066ff;
      --btn-bg-hover: #0051cc;
      --btn-text: #fff;
      --btn-radius: 10px;
      --btn-padding: 0.7rem 1.1rem;
      --btn-shadow: 0 6px 18px rgba(2,6,23,0.12);
      --btn-transition: 180ms cubic-bezier(.2,.9,.3,1);
      --focus-ring: 3px solid rgba(0,102,255,0.2);
      --font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }

    /* Reset & layout */
    *{box-sizing: border-box}
    html,body{height:100%}
    body{
      margin:0;
      display:grid;
      place-items:center;
      font-family:var(--font-family);
      background: #f6f9ff;
      padding:2rem;
    }

    /* Link button style (anchor styled as button) */
    .link-button{
      display:inline-flex;
      align-items:center;
      gap:0.6rem;
      text-decoration:none;
      background:var(--btn-bg);
      color:var(--btn-text);
      padding:var(--btn-padding);
      border-radius:var(--btn-radius);
      box-shadow:var(--btn-shadow);
      transition: transform var(--btn-transition), box-shadow var(--btn-transition), background-color var(--btn-transition);
      font-weight:600;
      font-size:1rem;
      line-height:1;
      border: none;
      cursor: pointer;
      user-select: none;
    }

    .link-button svg{
      width:1rem;
      height:1rem;
      flex-shrink:0;
      transform: translateX(0);
      transition: transform var(--btn-transition);
      stroke: currentColor;
      stroke-width: 1.4;
      fill: none;
    }

    .link-button:hover{
      background:var(--btn-bg-hover);
      transform: translateY(-3px);
      box-shadow: 0 10px 30px rgba(2,6,23,0.14);
    }

    .link-button:active{
      transform: translateY(0);
      box-shadow: 0 6px 18px rgba(2,6,23,0.12);
    }

    .link-button:focus{
      outline: none;
      box-shadow: var(--btn-shadow);
      position: relative;
    }

    /* visible focus ring for keyboard users */
    .link-button:focus-visible{
      box-shadow: var(--btn-shadow);
      border-radius: var(--btn-radius);
    }
    .link-button:focus-visible::after{
      content: "";
      position: absolute;
      inset: -6px;
      border-radius: calc(var(--btn-radius) + 6px);
      pointer-events: none;
      box-shadow: 0 0 0 6px rgba(0,102,255,0.09);
    }

    /* small animation: move icon on hover */
    .link-button:hover svg{
      transform: translateX(3px);
    }

    /* subtle accessible label styling */
    .sr-only{
      position:absolute!important;
      height:1px;width:1px;
      overflow:hidden;clip:rect(1px,1px,1px,1px);
      white-space:nowrap;border:0;padding:0;margin:-1px;
    }

    /* responsive tweak */
    @media (prefers-reduced-motion: reduce){
      .link-button, .link-button svg { transition: none; }
    }
  </style>
</head>
<body>

  <!--
    Use:
    - href: the URL you want the button to open
    - target="_blank" opens in a new tab; include rel="noopener noreferrer" for security
    - aria-label can be used to provide an explicit accessible name if needed
  -->
  <a
    class="link-button"
    href="<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Live Link Button</title>
  <style>
    :root{
      --btn-bg: #0066ff;
      --btn-bg-hover: #0051cc;
      --btn-text: #fff;
      --btn-radius: 10px;
      --btn-padding: 0.7rem 1.1rem;
      --btn-shadow: 0 6px 18px rgba(2,6,23,0.12);
      --btn-transition: 180ms cubic-bezier(.2,.9,.3,1);
      --focus-ring: 3px solid rgba(0,102,255,0.2);
      --font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }

    /* Reset & layout */
    *{box-sizing: border-box}
    html,body{height:100%}
    body{
      margin:0;
      display:grid;
      place-items:center;
      font-family:var(--font-family);
      background: #f6f9ff;
      padding:2rem;
    }

    /* Link button style (anchor styled as button) */
    .link-button{
      display:inline-flex;
      align-items:center;
      gap:0.6rem;
      text-decoration:none;
      background:var(--btn-bg);
      color:var(--btn-text);
      padding:var(--btn-padding);
      border-radius:var(--btn-radius);
      box-shadow:var(--btn-shadow);
      transition: transform var(--btn-transition), box-shadow var(--btn-transition), background-color var(--btn-transition);
      font-weight:600;
      font-size:1rem;
      line-height:1;
      border: none;
      cursor: pointer;
      user-select: none;
    }

    .link-button svg{
      width:1rem;
      height:1rem;
      flex-shrink:0;
      transform: translateX(0);
      transition: transform var(--btn-transition);
      stroke: currentColor;
      stroke-width: 1.4;
      fill: none;
    }

    .link-button:hover{
      background:var(--btn-bg-hover);
      transform: translateY(-3px);
      box-shadow: 0 10px 30px rgba(2,6,23,0.14);
    }

    .link-button:active{
      transform: translateY(0);
      box-shadow: 0 6px 18px rgba(2,6,23,0.12);
    }

    .link-button:focus{
      outline: none;
      box-shadow: var(--btn-shadow);
      position: relative;
    }

    /* visible focus ring for keyboard users */
    .link-button:focus-visible{
      box-shadow: var(--btn-shadow);
      border-radius: var(--btn-radius);
    }
    .link-button:focus-visible::after{
      content: "";
      position: absolute;
      inset: -6px;
      border-radius: calc(var(--btn-radius) + 6px);
      pointer-events: none;
      box-shadow: 0 0 0 6px rgba(0,102,255,0.09);
    }

    /* small animation: move icon on hover */
    .link-button:hover svg{
      transform: translateX(3px);
    }

    /* subtle accessible label styling */
    .sr-only{
      position:absolute!important;
      height:1px;width:1px;
      overflow:hidden;clip:rect(1px,1px,1px,1px);
      white-space:nowrap;border:0;padding:0;margin:-1px;
    }

    /* responsive tweak */
    @media (prefers-reduced-motion: reduce){
      .link-button, .link-button svg { transition: none; }
    }
  </style>
</head>
<body>

  <!--
    Use:
    - href: the URL you want the button to open
    - target="_blank" opens in a new tab; include rel="noopener noreferrer" for security
    - aria-label can be used to provide an explicit accessible name if needed
  -->
  <a
    class="link-button"
    href="https://example.com"
    target="_blank"
    rel="noopener noreferrer"
    aria-label="Open Example.com (opens in new tab)"
  >
    Visit Example
    <!-- simple arrow icon (SVG) -->
    <svg viewBox="0 0 24 24" aria-hidden="true" focusable="false">
      <path d="M5 12h14M13 5l6 7-6 7" stroke-linecap="round" stroke-linejoin="round"/>
    </svg>
  </a>

  <!-- hidden helper text for screen readers if you prefer -->
  <span class="sr-only">This button opens example.com in a new tab.</span>

</body>
</html>

    target="_blank"
    rel="noopener noreferrer"
    aria-label="Open Example.com (opens in new tab)"
  >
    Visit Example
    <!-- simple arrow icon (SVG) -->
    <svg viewBox="0 0 24 24" aria-hidden="true" focusable="false">
      <path d="M5 12h14M13 5l6 7-6 7" stroke-linecap="round" stroke-linejoin="round"/>
    </svg>
  </a>

  <!-- hidden helper text for screen readers if you prefer -->
  <span class="sr-only">This button opens example.com in a new tab.</span>

</body>
</html>
