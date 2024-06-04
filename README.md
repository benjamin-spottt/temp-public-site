# Snippet ref

```html
<style>
  #planexpo_iframe {
    height: calc(100vh - 60px);
    width: 100%;
  }
</style>
<iframe id="planexpo_iframe" style="border: none;"></iframe>
<script>
  var script = `
      <div id="planexpo-plan"></div>
        <script id="planHelper" src="https://<CLOUDFRONT-DOMAINNAME-DISTRIBUTION-PREFIX>.cloudfront.net/plan/<EVENT>/liveDataHelper.js"
        data-root-url="https://<CLOUDFRONT-DOMAINNAME-DISTRIBUTION-PREFIX>.cloudfront.net/<EVENT>/api/public_plan" data-source="dynamic" data-version="5"><\/script>
`;
  document.querySelector("#planexpo_iframe").contentDocument.write(script);
  document.querySelector("#planexpo_iframe").contentDocument.close();
</script>
```
