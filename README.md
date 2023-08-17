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
### Status Akun yang Verified
<p align='justify'>Status akun yang sudah teridentifikasi Verified sebesar 8 dan yang belum sebesar 92. Hal ini menjadi pertanyaan besar dikarenakan menurut data jumlah akun yang berstatus verified memposting lebih sedikit ketimbang akun yang belum verified. Pada jumlah postingan akun yang memiliki status verified sebesar 1293 postingan sedangkan akun yang tidak memiliki status verified sebesar 2400 postingan. Berdasarkan akun Eveline95 telah memposting sebesar 2400 postingan dan belum statusnya belum verified.</p>
<table>
  <tr>
      <td>
      <img src="https://github.com/kartikajls/InstagramAnalyze/assets/98092595/0122aeeb-ec97-42b3-82b7-a5a6c5648d7e"></img>
      </td>
      <td valign="top">
      <img src="https://github.com/kartikajls/InstagramAnalyze/assets/98092595/85e58cd3-833d-4b72-b441-66128849aec0"></img>
      </td>
  </tr>
</table>
<p align='justify'>Kemudian untuk akun yang berstatus private sebesar 50 akun dan tidak sebesar 50 akun.</p>
<img src="https://github.com/kartikajls/InstagramAnalyze/assets/98092595/0e137580-9472-4a53-81a4-8b9e1f792ce2"></img>

## Kesimpulan
<p align='justify'>Terdapat akun yang sudah berstatus verified sebesar 9 akun dan memiliki jumlah postingan sebesar 1293.</p>

## Kekurangan
<p align='justify'>Data instagram yang disajikan oleh kaggle.com masih belum lengkap sehingga insight yang diperoleh belum cukup untuk bisa menggambarkan keadaan database. Oleh karena itu penulis hanya bisa menyajikan sedikit informasi atau insight yang terkandung dalam database tersebut.</p>
