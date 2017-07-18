---
title: Grid
description: Components
layout: "guide"
weight: 100
---

<article id="1">

<div class="alert alert-warning clay-site-grid-width">
    <span class="clay-site-grid-width-sm">container-fluid-max-sm: 540px</span>
    <span class="clay-site-grid-width-md">container-fluid-max-md: 720px</span>
    <span class="clay-site-grid-width-lg">container-fluid-max-lg: 960px</span>
    <span class="clay-site-grid-width-xl">container-fluid-max-xl: 1140px</span>
    <span class="clay-site-grid-width-xxl">container-fluid-max-xxl: 1280px</span>
</div>

### Container Fluid

> Use classes <code class="code">container-fluid-max-sm</code>, <code class="code">container-fluid-max-md</code>, <code class="code">container-fluid-max-lg</code>, <code class="code">container-fluid-max-xl</code>, and <code class="code">container-fluid-max-xxl</code> in conjunction with <code class="code">container-fluid</code> to create containers that expand to 100% width, but don't expand beyond a set width e.g 1280px.

<div class="clay-site-container-fluid-switcher">
	<button class="btn btn-info" data-container-classes="container-fluid container-fluid-max-sm content" type="button">container-fluid-max-sm (540px)</button>
	<button class="btn btn-info" data-container-classes="container-fluid container-fluid-max-md content" type="button">container-fluid-max-md (720px)</button>
	<button class="btn btn-info" data-container-classes="container-fluid container-fluid-max-lg content" type="button">container-fluid-max-lg (960px)</button>
	<button class="btn btn-info" data-container-classes="container-fluid container-fluid-max-xl content" type="button">container-fluid-max-xl (1140px)</button>
	<button class="btn btn-info" data-container-classes="container-fluid container-fluid-max-xxl content" type="button">container-fluid-max-xxl (1280px)</button>
	<button class="btn btn-info" data-container-classes="container content" type="button">reset</button>
</div>

<script>
{literal}
$('.clay-site-container-fluid-switcher .btn').on('click', function(event) {
    var container = $('.content');
    console.log(container);
    var data = $(this).data('container-classes');
    consoel.log(data);
    container.attr('class', '');
    container.addClass(data);
});
{/literal}
</script>

</article>