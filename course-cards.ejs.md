```{=html}
<div class="amr-course-grid" style="--course-columns: <%- templateParams['grid-columns'] %>">
<% for (const item of items) { %>
  <article class="amr-course-card" aria-label="<%- item.title %>">
    <img class="amr-course-image"
         src="<%- item.image || '/images/r4beginners_1.png' %>"
         alt="<%- item.title %>">
    <div class="amr-course-footer" dir="rtl" lang="ar">
      <p class="amr-course-status">Registration Closed</p>
      <div class="amr-course-actions">
        <a href="<%- item.path %>"><span>Course Details</span><svg aria-hidden="true" viewBox="0 0 24 24"><path d="M19 12H5m6-6-6 6 6 6"/></svg></a>
        <a class="amr-course-pay" href="<%- templateParams['payment-url'] %>"><span>Course Materials</span><svg aria-hidden="true" viewBox="0 0 24 24"><path d="M19 12H5m6-6-6 6 6 6"/></svg></a>
      </div>
    </div>
  </article>
<% } %>
</div>
```
