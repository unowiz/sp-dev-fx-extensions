# Samples by Extension Type

Filter the samples by type of extension

 <div class="well">
  <div class="button-group filters-button-group">
    <button class="button is-checked" data-filter="*">All</button>
    <button class="button" data-filter="[data-type='Application']">Application Customizer</button>
    <button class="button" data-filter="[data-type='Command']">Listview Command Set</button>
    <button class="button" data-filter="[data-type='Field']">Field Customizer</button>
  </div>

</div>

<div class="grid">

{% for sample in samples|sort(attribute='modified', reverse=True) %}

<div class="sample-item" data-framework="{{sample.framework}}" data-spfx="{{sample.spfx}}" data-year="{{sample.year}}" data-modified="{{sample.modified}}" data-title="{{ sample.title }}" data-type="{{ sample.type }}" data-thumbnail="{{sample.thumbnail}}">
  <div class="sample">
    <div class="sample-video"><i class="ms-Icon ms-Icon--VideoSolid" aria-hidden="true"></i></div>
    <div class="sample-img">
      <a class="sample-link"
        href="{{sample.url}}"
        title="{{sample.title}}">
        <picture>
          <img src="../../img/thumbnails/sm/{{ sample.name }}.png" width="302" alt="{{sample.name}}" data-fullsize="{{sample.thumbnail}}" data-orig="../../img/thumbnails/sm/{{ sample.name }}.png"/>
        </picture>
      </a>
    </div>
  </div>
      <a href="{{sample.url}}"
      title="{{ sample.title }}">
<span class="location" title="Framework: {{sample.framework}}">{{ sample.framework }}</span>
  <h2 class="name">
      {{sample.title}}</h2>
      <div class="sample-activity">
  <span class="author" title="{{ sample.author }}">{{ sample.author }}</span>
  <span class="modified">Modified {{ sample.modifiedtext }}</span>
  </div>
  </a>

</div>
    {% endfor %}
</div>

<img src="https://telemetry.sharepointpnp.com/sp-dev-fx-extensions/docs/samples/framework" />