Accessibility Checker Pass Test Advices
***

1. Use <strong> instead </b>.
2. Use <em> instead <i>.
3. Each form input (input, select, textarea, etc) should have label with text and for="" attribute with input's id:
<div class="form-group">
	<label for="input-id">Label Text</label>
	<input type="text" id="input-id">
</div>

If label should be invisible use class="visually-hidden":
<label for="input-id" class="visually-hidden">Label Text</label>
It will be visible for screenreaders only.

4. Headers in page should go from bigger to smaller:
h1, then h2, then h3 etc...
Use these advices when test:
https://www.w3.org/WAI/GL/WCAG20/tests/test38.html






