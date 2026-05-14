<table class="table table-hover responsibe">
  <thead>
    <tr>
      <th scope="col">Date</th>
      <th scope="col">Certification</th>
      <th scope="col">Issuer</th>
      <th scope="col">Link</th>
    </tr>
  </thead>
  <tbody>
    {% for cert in site.data.certifications %} 
    <tr>
      <td>{{ cert.date }}</td>
      <td><strong>{{ cert.title }}</strong></td>
      <td>{{ cert.issuer }}</td>
      <td>[View]({{ cert.link }})
      </td>
    </tr>
    {% endfor %}
  </tbody>
</table>