# Instagram dataset Analyze
<p align='justify'>Instagram merupakan platform terbesar didunia setelah facebook. Dalam penggunaannya, instagram memiliki fitur kegunaan dan fungsi masing-masing. Hal ini yang menjadikan informasi yang terkandung disetiap aktivitas instagram tercatat dan membentuk sebuah data yang sangat besar. Pada kesempatan ini, kaggle.com telah memperbarui datanya yang berjudul "instagram dataset". Oleh karena itu penulis dari akun github ini akan menganalisa dan menggali insight yang terkandung didalam data tersebut.</p>

## Preparation Data
<p align='justify'>Pada tahapan ini yaitu mempersiapkan data yang ingin dianalisis, data tersebut adalah comments.csv, follows.csv, likes.csv, photo_tags.csv, photo.csv, tags.csv, users.csv. Load data tersebut yang hasilnya akan seperti gambar dibawah ini.</p>

#### Comments
<img src="https://github.com/kartikajls/InstagramAnalyze/assets/98092595/46735ce9-96ce-4758-a484-2ec8175f21ed"></img>
#### Follows
<img src="https://github.com/kartikajls/InstagramAnalyze/assets/98092595/2eacb133-3f29-41b3-ba31-db4f3ad5ac47"></img>
#### Likes
<img src="https://github.com/kartikajls/InstagramAnalyze/assets/98092595/a4277cc7-b874-47ca-8c7e-39f6c4ac0072"></img>
#### Photo tags
<img src="https://github.com/kartikajls/InstagramAnalyze/assets/98092595/8b0cf3f0-ec39-41a6-9f5b-ca2608e12b6c"></img>
##### Photos
<img src="https://github.com/kartikajls/InstagramAnalyze/assets/98092595/f14a3775-7138-4ad9-b8dd-0e8ba4c2a286"></img>
#### Tags
<img src="https://github.com/kartikajls/InstagramAnalyze/assets/98092595/d76b2f8d-f3ff-42c6-9d27-7c2d5ce71793"></img>
#### Users
<img src="https://github.com/kartikajls/InstagramAnalyze/assets/98092595/2cec4307-3ca8-41d9-afa7-519d1bacb8dc"></img>

## Cleansing Data
<p align='justify'>Pada tahap ini, terdapat data yang harus "dimanipulasi", tujuannya adalah untuk bisa di teliti terlebih dahulu. Data tersebut yaitu data follows, dimana keterangan untuk akun yang berstatus private ada penulisan yang berbeda. Oleh karena itu harus disamakan dengan cara membuat data frame baru untuk data follows.</p>
<table>
  <tr>
    <td>
      df_new_follows = df_follows.replace('Private', 'private')
    </td>
  </tr>
</table>

## Exploratory Data
