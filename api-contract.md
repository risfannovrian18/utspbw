# Guru

### <b>Create Guru (POST)</b>

<details>
<summary> Klik untuk ekspand </summary>
<table>
<tr>
    <td> URL </td>
    <td> {{baseURL}}/api/v1/Guru </td>
</tr>
<tr>
    <td> Method </td>
    <td> POST </td>
</tr>
<tr>
    <td> <b> Header </b></td>
    <td> Authorization : Bearer Token </td>
</tr>
<tr>
    <td> <b> Body </b></td>
    <td>

```json
{
  "nama": "Ernawati",
  "alamat": "Bogor",
  "hobi": "Membaca"
}
```

</td>
</tr>

<tr>
    <td> <b> Respon Success </b></td>
    <td>

```json
{
  "code": 201,
  "message": "Data Guru Berhasil diinput",
  "data": {
    "id": 1234,
    "nama": "Ernawati",
    "alamat": "Bogor",
    "hobi": "Membaca"
  }
}
```

</td>
</tr>

<tr>
    <td> <b> Respon Conflict </b></td>
    <td>

```json
{
  "code": 409,
  "message": "Nama Guru Telah digunakan",
  "data": {
    "value": "Ernawati",
    "property": "nama",
    "location": "body"
  }
}
```

</td>
</tr>

</table>
</details>

### <b>Read Guru by Id (GET)</b>

<details>
<summary> Klik untuk ekspand </summary>

<table>
<tr>
    <td> URL </td>
    <td> {{baseURL}}/api/v1/Guru </td>
</tr>
<tr>
    <td> EXAMPLE </td>
    <td> {{baseURL}}/api/v1/Guru?id=1234 </td>
</tr>
<tr>
    <td> Method </td>
    <td> GET </td>
</tr>
<tr>
    <td> <b> Header </b></td>
    <td> Authorization : Bearer Token </td>
</tr>
<tr>
    <td> <b> Query </b></td>
    <td> id=1234 </td>
</tr>

<tr>
    <td> <b> Respon Success With Query </b></td>
    <td>

```json
{
  "code": 200,
  "message": "Data Guru Berhasil diinput",
  "data": {
    "nama": "Ernawati",
    "alamat": "Bogor",
    "hobi": "Membaca"
  }
}
```

</td>
</tr>

<tr>
    <td> <b> Respon Not Found </b></td>
    <td>

```json
{
  "code": 404,
  "message": "ID Guru tidak ditemukan",
  "data": {
    "value": "1234",
    "property": "id",
    "location": "query"
  }
}
```

</td>
</tr>
</table>
</details>

### <b>Read Guru All (GET)</b>

<details>
<summary> Klik untuk ekspand </summary>

<table>
<tr>
    <td> URL </td>
    <td> {{baseURL}}/api/v1/Guru </td>
</tr>

<tr>
    <td> Method </td>
    <td> GET </td>
</tr>
<tr>
    <td> <b> Header </b></td>
    <td> Authorization : Bearer Token </td>
</tr>

<tr>
    <td> <b> Respon Success </b></td>
    <td>

```json
{
  "code": 200,
  "message": "Sukses",
  "data": [
    {
      "id": 1234,
      "nama": "Ernawati",
      "alamat": "Bogor",
      "hobi": "Membaca"
    },
    {
      "id": 1235,
      "nama": "Fendra",
      "alamat": "Jakarta",
      "hobi": "Olahraga"
    }
  ]
}
```

</td>
</tr>

<tr>
    <td> <b> Respon Not Found </b></td>
    <td>

```json
{
  "code": 404,
  "message": "ID Guru tidak ditemukan",
  "data": {
    "value": "1234",
    "property": "id",
    "location": "query"
  }
}
```

</td>
</tr>
</table>
</details>

### <b>Update Guru (PUT)</b>

<details>
<summary> Klik untuk ekspand </summary>

<table>
<tr>
    <td> URL </td>
    <td> {{baseURL}}/api/v1/Guru </td>
</tr>
<tr>
    <td> Method </td>
    <td> PUT </td>
</tr>
<tr>
    <td> <b> Header </b></td>
    <td> Authorization : Bearer Token </td>
</tr>
<tr>
    <td> <b> Body </b></td>
    <td>

```json
{
  "id": 1234,
  "nama": "Ernawati Hana",
  "alamat": "Bogor",
  "hobi": "Menulis"
}
```

</td>
</tr>

<tr>
    <td> <b> Respon Success </b></td>
    <td>

```json
{
  "code": 201,
  "message": "Data Guru Berhasil diubah",
  "data": {
    "id": 1234,
    "nama": "Ernawati Hana",
    "alamat": "Bogor",
    "hobi": "Menulis"
  }
}
```

</td>
</tr>

<tr>
    <td> <b> Respon Conflict </b></td>
    <td>

```json
{
  "code": 409,
  "message": "Nama Guru Telah digunakan",
  "data": {
    "value": "Ernawati Hana",
    "property": "nama",
    "location": "body"
  }
}
```

</td>
</tr>

<tr>
    <td> <b> Respon Not Found </b></td>
    <td>

```json
{
  "code": 404,
  "message": "ID Guru tidak ditemukan",
  "data": {
    "value": "1234",
    "property": "id",
    "location": "body"
  }
}
```

</td>
</tr>

</table>
</details>

### <b>Delete Guru (DELETE)</b>

<details>
<summary> Klik untuk ekspand </summary>

<table>
<tr>
    <td> URL </td>
    <td> {{baseURL}}/api/v1/Guru </td>
</tr>
<tr>
    <td> EXAMPLE </td>
    <td> {{baseURL}}/api/v1/Guru?id=1234 </td>
</tr>
<tr>
    <td> Method </td>
    <td> DELETE </td>
</tr>
<tr>
    <td> <b> Header </b></td>
    <td> Authorization : Bearer Token </td>
</tr>
<tr>
    <td> <b> Query </b></td>
    <td> id=1234 </td>
</tr>

<tr>
    <td> <b> Respon Success</b></td>
    <td>

```json
{
  "code": 200,
  "message": "Data Guru Berhasil dihapus",
  "data": []
}
```

</td>
</tr>

<tr>
    <td> <b> Respon Not Found </b></td>
    <td>

```json
{
  "code": 404,
  "message": "ID Guru tidak ditemukan",
  "data": {
    "value": "1234",
    "property": "id",
    "location": "query"
  }
}
```

</td>
</tr>
</table>
</details>
</br></br>

# Staff

### <b>Create Staff (POST)</b>

<details>
<summary> Klik untuk ekspand </summary>

<table>
<tr>
    <td> URL </td>
    <td> {{baseURL}}/api/v1/Staff </td>
</tr>
<tr>
    <td> Method </td>
    <td> POST </td>
</tr>
<tr>
    <td> <b> Header </b></td>
    <td> Authorization : Bearer Token </td>
</tr>
<tr>
    <td> <b> Body </b></td>
    <td>

```json
{
  "nama": "Arif",
  "alamat": "Bogor",
  "hobi": "Panahan"
}
```

</td>
</tr>

<tr>
    <td> <b> Respon Success </b></td>
    <td>

```json
{
  "code": 201,
  "message": "Data Staff Berhasil diinput",
  "data": {
    "id": 1235,
    "nama": "Arif",
    "alamat": "Bogor",
    "hobi": "Panahan"
  }
}
```

</td>
</tr>

<tr>
    <td> <b> Respon Conflict </b></td>
    <td>

```json
{
  "code": 409,
  "message": "Nama Staff Telah digunakan",
  "data": {
    "value": "Arif",
    "property": "nama",
    "location": "body"
  }
}
```

</td>
</tr>

</table>
</details>

### <b>Read Staff by Id (GET)</b>

<details>
<summary> Klik untuk ekspand </summary>

<table>
<tr>
    <td> URL </td>
    <td> {{baseURL}}/api/v1/Staff </td>
</tr>
<tr>
    <td> EXAMPLE </td>
    <td> {{baseURL}}/api/v1/Staff?id=1235 </td>
</tr>
<tr>
    <td> Method </td>
    <td> GET </td>
</tr>
<tr>
    <td> <b> Header </b></td>
    <td> Authorization : Bearer Token </td>
</tr>
<tr>
    <td> <b> Query </b></td>
    <td> id=1235 </td>
</tr>

<tr>
    <td> <b> Respon Success With Query </b></td>
    <td>

```json
{
  "code": 200,
  "message": "Data Staff Berhasil diinput",
  "data": {
    "nama": "Arif",
    "alamat": "Bogor",
    "hobi": "Panahan"
  }
}
```

</td>
</tr>

<tr>
    <td> <b> Respon Not Found </b></td>
    <td>

```json
{
  "code": 404,
  "message": "ID Staff tidak ditemukan",
  "data": {
    "value": "1235",
    "property": "id",
    "location": "query"
  }
}
```

</td>
</tr>
</table>
</details>

### <b>Read Staff All (GET)</b>

<details>
<summary> Klik untuk ekspand </summary>

<table>
<tr>
    <td> URL </td>
    <td> {{baseURL}}/api/v1/Staff </td>
</tr>

<tr>
    <td> Method </td>
    <td> GET </td>
</tr>
<tr>
    <td> <b> Header </b></td>
    <td> Authorization : Bearer Token </td>
</tr>

<tr>
    <td> <b> Respon Success </b></td>
    <td>

```json
{
  "code": 200,
  "message": "Sukses",
  "data": [
    {
      "id": 1235,
      "nama": "Arif",
      "alamat": "Bogor",
      "hobi": "Panahan"
    },
    {
      "id": 1236,
      "nama": "Ajang",
      "alamat": "Bogor",
      "hobi": "Tidur"
    }
  ]
}
```

</td>
</tr>

<tr>
    <td> <b> Respon Not Found </b></td>
    <td>

```json
{
  "code": 404,
  "message": "ID Staff tidak ditemukan",
  "data": {
    "value": "1235",
    "property": "id",
    "location": "query"
  }
}
```

</td>
</tr>
</table>
</details>

### <b>Update Staff (PUT)</b>

<details>
<summary> Klik untuk ekspand </summary>

<table>
<tr>
    <td> URL </td>
    <td> {{baseURL}}/api/v1/Staff </td>
</tr>
<tr>
    <td> Method </td>
    <td> PUT </td>
</tr>
<tr>
    <td> <b> Header </b></td>
    <td> Authorization : Bearer Token </td>
</tr>
<tr>
    <td> <b> Body </b></td>
    <td>

```json
{
  "id": 1235,
  "nama": "Arif Hidayat",
  "alamat": "Bogor",
  "hobi": "E-Panahan"
}
```

</td>
</tr>

<tr>
    <td> <b> Respon Success </b></td>
    <td>

```json
{
  "code": 201,
  "message": "Data Staff Berhasil diubah",
  "data": {
    "id": 1235,
    "nama": "Arif Hidayat",
    "alamat": "Bogor",
    "hobi": "Panahan"
  }
}
```

</td>
</tr>

<tr>
    <td> <b> Respon Conflict </b></td>
    <td>

```json
{
  "code": 409,
  "message": "Nama Staff Telah digunakan",
  "data": {
    "value": "Arif Hidayat",
    "property": "nama",
    "location": "body"
  }
}
```

</td>
</tr>

<tr>
    <td> <b> Respon Not Found </b></td>
    <td>

```json
{
  "code": 404,
  "message": "ID Staff tidak ditemukan",
  "data": {
    "value": "1235",
    "property": "id",
    "location": "body"
  }
}
```

</td>
</tr>

</table>
</details>

### <b>Delete Staff (DELETE)</b>

<details>
<summary> Klik untuk ekspand </summary>

<table>
<tr>
    <td> URL </td>
    <td> {{baseURL}}/api/v1/Staff </td>
</tr>
<tr>
    <td> EXAMPLE </td>
    <td> {{baseURL}}/api/v1/Staff?id=1235 </td>
</tr>
<tr>
    <td> Method </td>
    <td> DELETE </td>
</tr>
<tr>
    <td> <b> Header </b></td>
    <td> Authorization : Bearer Token </td>
</tr>
<tr>
    <td> <b> Query </b></td>
    <td> id=5 </td>
</tr>

<tr>
    <td> <b> Respon Success</b></td>
    <td>

```json
{
  "code": 200,
  "message": "Data Staff Berhasil dihapus",
  "data": []
}
```

</td>
</tr>

<tr>
    <td> <b> Respon Not Found </b></td>
    <td>

```json
{
  "code": 404,
  "message": "ID Staff tidak ditemukan",
  "data": {
    "value": "1235",
    "property": "id",
    "location": "query"
  }
}
```

</td>
</tr>
</table>
</details>
