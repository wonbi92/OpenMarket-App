# ๐ฃ Open Market 
- Gundy์ Wonbi๊ฐ ๋ง๋  Open Market App์๋๋ค.

## ๐ ๋ชฉ์ฐจ
1. [ํ ์๊ฐ](#-ํ-์๊ฐ)
2. [ํ ์ํค](#-ํ-์ํค)
3. [์คํ ํ๋ฉด](#-์คํ-ํ๋ฉด)
4. [Diagram](#-diagram)
5. [ํด๋ ๊ตฌ์กฐ](#-ํด๋-๊ตฌ์กฐ)
6. [ํ์๋ผ์ธ](#-ํ์๋ผ์ธ)
7. [๊ธฐ์ ์  ๋์ ](#-๊ธฐ์ ์ -๋์ )
8. [ํธ๋ฌ๋ธ ์ํ ๋ฐ ๊ณ ๋ฏผ](#-ํธ๋ฌ๋ธ-์ํ-๋ฐ-๊ณ ๋ฏผ)
9. [์ฐธ๊ณ  ๋งํฌ](#-์ฐธ๊ณ -๋งํฌ)


## ๐ฑ ํ ์๊ฐ
|[Wonbi](https://github.com/wonbi92)|[Gundy](https://github.com/Gundy93)|
|:---:|:---:|
| <img width="180px" img style="border: 2px solid lightgray; border-radius: 90px;-moz-border-radius: 90px;-khtml-border-radius: 90px;-webkit-border-radius: 90px;" src="https://avatars.githubusercontent.com/u/88074999?v=4">| <img width="180px" img style="border: 2px solid lightgray; border-radius: 90px;-moz-border-radius: 90px;-khtml-border-radius: 90px;-webkit-border-radius: 90px;" src= "https://avatars.githubusercontent.com/u/106914201?v=4">|

## ๐งญ ํ ์ํค

#### [๐ค Ground Rule](https://github.com/wonbi92/ios-open-market/wiki/1.-Ground-Rule)

#### [๐ Code Convention](https://github.com/wonbi92/ios-open-market/wiki/2.-Code-Convention)

#### [๐ ์ผ์ผ ์คํฌ๋ผ](https://github.com/wonbi92/ios-open-market/wiki/3.-Open-Market-Scrum)

## ๐  ์คํ ํ๋ฉด

|์ํ ๋ฑ๋กํ๊ธฐ|์ํ ์์ ํ๊ธฐ|์ํ ์ญ์ ํ๊ธฐ|
|:-:|:-:|:-:|
|![](https://i.imgur.com/zcV7Vog.gif)|![](https://i.imgur.com/eFOJ40b.gif)|![](https://i.imgur.com/qrtF3n9.gif)|
|**์คํฌ๋กคํ๊ธฐ**|**๋ฆฌ์คํธ ๊ทธ๋ฆฌ๋ ์ค์์นํ๊ธฐ**|**๋ฆฌํ๋ ์ํ๊ธฐ**|
|![](https://i.imgur.com/UdF51GR.gif)|![](https://i.imgur.com/ffuak0c.gif)|![](https://i.imgur.com/INfTQJZ.gif)|

## ๐ Diagram

### ๐งฌ Class Diagram
![](https://i.imgur.com/PIlQgev.png)

 
## ๐ ํด๋ ๊ตฌ์กฐ
> Network: ์๋ฒ๋ก๋ถํฐ ๋ฐ์ดํฐ๋ฅผ ๋ฐ์์ค๋ ๋ก์ง์ ๋ด๋น <br>
> OpenMarket: ๋ฐ์ดํฐ๋ฅผ ์ฒ๋ฆฌํ๊ณ  ์ปจํธ๋กค ํ๋ ๋ฉ์ธ ๊ตฌ์กฐ <br>
> Extension: ๊ธฐ์กด ํ์์ ์ปค์คํ ๋ก์ง ์ถ๊ฐ<br>
> OpenMarketTests: ์ ๋ ํ์คํธ
```
OpenMarket
โโโ AppDelegate
โโโ SceneDelegate
โโโ Extension
โย ย  โโโ Collection+
โย ย  โโโ Data+
โย ย  โโโ DecodingError+
โย ย  โโโ Int+
โย ย  โโโ JSONCoder+
โย ย  โโโ UIImage+
โโโ Network
โย ย  โโโ Network Protocol
โย ย  โย ย  โโโ URLSessionDataTaskProtocol
โย ย  โย ย  โโโ URLSessionProtocol
โย ย  โโโ HttpMethod
โย ย  โโโ NetworkError
โย ย  โโโ NetworkManager
โย ย  โโโ NetworkRequest
โโโ OpenMarket
โย ย  โโโ ProductsViewController
โย ย  โโโ ProductManagingViewController
โย ย  โโโ AddProductViewController
โย ย  โโโ EditProductViewController
โย ย  โโโ ProductDetailViewController
โย ย  โโโ DetailView
โย ย  โโโ ListCell
โย ย  โโโ GridCell
โย ย  โโโ ImageCell
โย ย  โโโ DetailImageCell
โย ย  โโโ Model
โย ย  โย ย  โโโ Product
โย ย  โย ย  โโโ ProductList
โย ย  โย ย  โโโ DetailProduct
โย ย  โย ย  โโโ SendingProduct
โย ย  โโโ Network
โย ย  โย ย  โโโ ImageCacheManager
โย ย  โย ย  โโโ MultipartFormData
โย ย  โย ย  โโโ OpenMarketNetworkRequest
โย ย  โโโ FormatConverter
โโโ OpenMarketTests
 ย ย  โโโ JSONParsingTests
 ย ย  โโโ MockData
 ย ย  โย ย  โโโ DataLoader
 ย ย  โย ย  โโโ products
 ย ย  โโโ NetworkManagerTests
 ย ย  โโโ NetworkRequestTests
 ย ย  โโโ Test Double
 ย ย      โโโ DummyData
 ย ย      โโโ MockURLSession
 ย ย      โโโ MockURLSessionDataTask
```

## โฐ ํ์๋ผ์ธ

#### ๐ Step 1
- JSONParsing
    - โ DTO ์์ฑ
- Networking ๊ตฌํ
    - โ URLSession์ ํ์ฉํ ์๋ฒ์์ ๋ฐ์ดํฐ ํต์ 
    - โ ๊ฐ ๋คํธ์ํน ์์๋ฅผ ํ๋กํ ์ฝ์ ์ด์ฉํ์ฌ ์ถ์ํ
- Test Double ์์ฑ
    - โ ํ์คํธ๋ฅผ ์ํ ๊ฐ์ฒด ์์ฑ
    - โ Unit Test ์งํ

<details>
<summary> 
ํผ์ณ๋ณด๊ธฐ
</summary>
    
1๏ธโฃ **Network**
- HttpMethod 
    - HttpMethod๋ฅผ ๋ํ๋ด๋ ์ด๊ฑฐํ ํ์์๋๋ค.
- NetworkRequest
    - ๋คํธ์ํน์ ์ํ URL๊ณผ Request๋ฅผ ๊ฐ์ง๊ณ  ์ด๋ฅผ ๊ตฌํํ๊ธฐ ์ํ ํ์ ํ๋กํผํฐ๋ฅผ ์ ์ธํ๋ ํ๋กํ ์ฝ์๋๋ค.
- NetworkManager
    - ๋คํธ์ํฌ์์ ๋ฐ์ดํฐ๋ฅผ ๊ฐ์ ธ์ ์ค๋ฅ๋ฅผ ์ฒ๋ฆฌํ๊ณ  ๋ฐ์ดํฐ๋ฅผ ํ์ฑํด์ฃผ๋ ๊ฐ์ฒด์๋๋ค.
- URLSessionProtocol
    - DIP์ ์ฉ์ ์ํด `dataTask`๋ฉ์๋๋ฅผ ์ ์ํ๋ ํ๋กํ ์ฝ์๋๋ค.
    - ์ด ํ๋กํ ์ฝ์ ์ฑํํ๋ฉด `dataTask`๋ฉ์๋์ ๋ก์ง์ ๊ตฌํํด์ฃผ์ด์ผ ํฉ๋๋ค.
- URLSessionDataTaskProtocol
    - `URLSessionProtocol`์ `dataTask`๋ฉ์๋์์ ๋ฐํํ๋ ํ์์ ์ง์ ํ๋ ํ๋กํ ์ฝ์๋๋ค.
    - ์ด ํ๋กํ ์ฝ์ ์ฑํํ๋ฉด `resume`๋ฉ์๋์ ๋ก์ง์ ๊ตฌํํด์ฃผ์ด์ผ ํฉ๋๋ค.
     
2๏ธโฃ **Extension**
- JSONDecoder
    - ์ ๋ค๋ฆญ ํ์๊ณผ ๋ฐ์ดํฐ๋ฅผ ๋ฐ์ ๋์ฝ๋ฉํ๋ ํ์ ๋ฉ์๋๋ฅผ ์ถ๊ฐํ์์ต๋๋ค.
- String
    - `"yyyy-MM-dd'T'HH:mm:ss"`์ ํ์์ ๋ฌธ์์ด์ `Date`ํ์์ ๊ฐ์ผ๋ก ๋ณ๊ฒฝ์์ผ์ฃผ๋ ๋ฉ์๋๋ฅผ ์ถ๊ฐํ์์ต๋๋ค.

3๏ธโฃ **OpenMarket**
- Product
    - `Codable`์ ์ฑํํ๋ DTO์๋๋ค.
- ProductList
    - `Codable`์ ์ฑํํ๋ DTO์๋๋ค.
- HealthCheckerRequest
    - NetworkRequest๋ฅผ ์ฑํํ๊ณ , Application HealthChekcer๋ฅผ ๋ฆฌํ์คํธํ๊ธฐ์ํ ํ๋กํผํฐ๋ฅผ ๊ฐ๊ณ  ์๋ ๊ตฌ์กฐ์ฒด์๋๋ค.
- ProductListRequest
    - NetworkRequest๋ฅผ ์ฑํํ๊ณ , ์ํ ๋ฆฌ์คํธ ์กฐํ๋ฅผ ๋ฆฌํ์คํธํ๊ธฐ์ํ ํ๋กํผํฐ๋ฅผ ๊ฐ๊ณ  ์๋ ๊ตฌ์กฐ์ฒด์๋๋ค.
- ProductDetailRequest
    - NetworkRequest๋ฅผ ์ฑํํ๊ณ , ์ํ ์์ธ ์กฐํ๋ฅผ ๋ฆฌํ์คํธํ๊ธฐ์ํ ํ๋กํผํฐ๋ฅผ ๊ฐ๊ณ  ์๋ ๊ตฌ์กฐ์ฒด์๋๋ค.
    
    
4๏ธโฃ **Test Double**
- products
    - ํ์คํธ๋ฅผ ์ํ Mock JSON๋ฐ์ดํฐ์๋๋ค.
- DataLoader
    - Mock JSON๋ฐ์ดํฐ๋ฅผ ์ฝ๋๋ก ์ฐ๊ฒฐ์์ผ data๋ฅผ ์์ฑํด์ฃผ๋ ํด๋์ค์๋๋ค.
- DummyData
    - ์ค์  ๋คํธ์ํน์ด ์๋ ํ์คํธ๋ฅผ ์งํํ  ๋ ๋ฐํํ  ๋ฐ์ดํฐ ๊ตฌ์กฐ์ฒด์๋๋ค.
- MockURLSession
    - ํ์คํธ๋ฅผ ์ํด ์ค์  ๋คํธ์ํน์ด ์๋๋ผ `DummyData`๋ฅผ ์ฌ์ฉํ๋ ํด๋์ค์๋๋ค.
- MockURLSessionDataTask
    - ํ์คํธ๋ฅผ ์ํด ์ค์  ๋คํธ์ํน ํ์คํธ๊ฐ ์๋ `DummyData`๋ฅผ ๋ฐํํ๋ ํด๋์ค ์๋๋ค.
    
5๏ธโฃ **Unit Test**
- JSONDecoder, DTO
    - JSONParsingTests
- NetworkManager
    - NetworkManagerTests
- OpenMarketNetworkRequest
    - NetworkRequestTests
</details>

#### ๐ Step 2
- ์ปฌ๋ ์ ๋ทฐ ์ฌ์ฉํ๊ธฐ
    - โ ์ปค์คํฐ๋ง์ด์ง ์ ๊ตฌํํ๊ธฐ
    - โ ๋ฆฌ์คํธ์ ๊ทธ๋ฆฌ๋ ๋ชจ์์ ์ปฌ๋ ์ ๋ทฐ ๊ตฌํํ๊ธฐ
- ์ด๋ฏธ์ง ๋น๋๊ธฐ๋ก ์ฒ๋ฆฌํ๊ธฐ
    - โ ์ด๋ฏธ์ง๋ฅผ ์๋ฒ์์ ํ์ฑํ๋ ๊ณผ์ ์ ๋น๋๊ธฐ๋ก ์ฒ๋ฆฌํ๊ธฐ
    - โ race condition ํด๊ฒฐํ๊ธฐ
- UISegmentedControl ์ฌ์ฉํ๊ธฐ
- ์ด๋ฏธ์ง ์บ์ฑํ๊ธฐ
    - โ ์๋ฒ๋ฅผ ํตํด์ ์ ๋ฌ๋ฐ์ ๋ฐ์ดํฐ๋ฅผ ๋ก์ปฌ์ ์บ์ํ๊ธฐ

<details>
<summary> 
ํผ์ณ๋ณด๊ธฐ
</summary>

1๏ธโฃ **Extension**
- DecodingError
    - `errorDescription`์ ์ฌ์ฉํด ์ํฉ์ ๋ง๋ ์๋ฌ ๋ฉ์ธ์ง๋ฅผ ์ถ๋ ฅํ๋๋ก ํ์์ต๋๋ค.
- Collection
    - `subscript`๋ฅผ ์ด์ฉํด ์ฒจ์ ๋ฌธ๋ฒ์ผ๋ก ๊ฐ์ ์ ๊ทผ ์ ๋ฐํ์์๋ฌ๊ฐ ๋์ง ์๋๋ก ํ์์ต๋๋ค.
- Int
    - ๊ฐ์ด 0์ธ์ง ํ์ธํ๋ `isZero`, ์ซ์์ ์๋ฆฌ์๋ฅผ ์ฒดํฌํ๋ `decimal` ํ๋กํผํฐ๋ฅผ ๊ฐ์ง๋๋ก ํ์์ต๋๋ค.
- OpenMarket
    - Product
        - ์ด์  `Product`๋ `Hashable`์ ์ฑํํฉ๋๋ค.
    - ImageCacheManager
        - ์ด๋ฏธ์ง๋ฅผ ์บ์ฑํ๊ธฐ ์ํ ์ฑ๊ธํค ๊ฐ์ฒด์๋๋ค.

2๏ธโฃ **Controller**
- ProductsViewController
    - ์ฑ ์คํ์ ๋์ค๋ ์ฒซ ํ๋ฉด์ ์ปจํธ๋กค ํฉ๋๋ค.
    - ๋ฐ์ดํฐ๋ฅผ ํ์ฑํ๊ณ  ์ด๋ฅผ ๊ฐ ์ปฌ๋ ์ ๋ทฐ์ ์ ๋ฌํฉ๋๋ค.
    - segmentedControl์ ๊ฐ์ด ๋ฐ๋ ๋ ๋ง๋ค ๊ฐ๊ฐ์ ์ปฌ๋ ์ ๋ทฐ๋ฅผ ๋ณด์ฌ์ฃผ๋๋ก ํ๋ฉด์ ์ ํํฉ๋๋ค.
- AddProductViewController
    - ๋ค์ ์คํ์์ ์ถ๊ฐ๋  ์๋ก์ด ์ํ์ ๋ฑ๋กํ๋ ํ๋ฉด์ ์ปจํธ๋กคํฉ๋๋ค.

3๏ธโฃ **View**
- ListCollectionViewCell
    - ๋ฆฌ์คํธ ํํ์ ์ปฌ๋ ์ ๋ทฐ์์ ์ฌ์ฉํ๋ ์์๋๋ค.
    - ๋ฆฌ์คํธ ํํ๋ก ์ปค์คํฐ๋ง์ด์ง ๋ ์์ ๊ทธ๋ฆฝ๋๋ค.
- GridCollectionViewCell
    - ๊ทธ๋ฆฌ๋ ํํ์ ์ปฌ๋ ์ ๋ทฐ์์ ์ฌ์ฉํ๋ ์์๋๋ค.
    - ๊ทธ๋ฆฌ๋ ํํ๋ก ์ปค์คํฐ๋ง์ด์ง ๋ ์์ ๊ทธ๋ฆฝ๋๋ค.
</details>

#### ๐ Step 3
- ์ปฌ๋ ์ ๋ทฐ ์ฌ์ฉํ๊ธฐ
    - โ ํ๋์ ์ปฌ๋ ์ ๋ทฐ์ ์ฌ๋ฌ๊ฐ์ FlowLayout์ ์ฉํ๊ธฐ
- ๋ชจ๋ ์ปฌ๋ ์ ๋ทฐ ์ฌ์ฉํ๊ธฐ
    - โ ์ปค์คํฐ๋ง์ด์ง ์ ๊ตฌํํ๊ธฐ
    - โ ๊ฐ๋ก ์คํฌ๋กค๋๋ ์ปฌ๋ ์๋ทฐ ๊ตฌํํ๊ธฐ
    - โ DiffableDataSource, Snapshot ํ์ฉํ๊ธฐ
- ๋คํธ์ํน
    - โ multipart/form-data httpBody ๋ง๋ค๊ธฐ
    - โ POST, DELETE httpMethod๋ฅผ ์์ฒญํ๋ Request ์์ฑํ๊ธฐ
    - โ UUID๋ฅผ ํ์ฉํ ๊ณ ์ ๊ฐ ํ ๋นํ๊ธฐ

<details>
<summary> 
ํผ์ณ๋ณด๊ธฐ
</summary>

1๏ธโฃ **Extension**
- Data
    - `append(_:using:)`์ ์ฌ์ฉํด ๋ฌธ์์ด์ Data ํ์์ผ๋ก ๋ณํ์์ผ ์ถ๊ฐํ๋๋ก ํ์์ต๋๋ค.

2๏ธโฃ **Controller**
- AddProductViewController
    - ์ํ์ ๋ฑ๋ก๊ณผ ์์ ์ ๋ด๋นํ๋ ๋ทฐ ์ปจํธ๋กค๋ฌ์๋๋ค.
    - ์ด๋ฏธ์ง๊ฐ ์ถ๊ฐ๋  ๋๋ง๋ค ์ด๋ฏธ์ง ์ปฌ๋ ์๋ทฐ์ ์์ดํ๋ ์ถ๊ฐ๋ฉ๋๋ค.

3๏ธโฃ **AddProductViewController**
- ImageCell
    - AddProductViewController์์ ์ํ์ ์ด๋ฏธ์ง๋ฅผ ๋ด๋นํ๋ ์์๋๋ค.

4๏ธโฃ **OpenMarket**
- EditProduct
    - Codable์ ์ฑํํ๋ DTO์๋๋ค.
    - ์ํ ์์ ์ ๋ณ๊ฒฝ๋  ๊ฐ์ ๊ฐ์ต๋๋ค.
- NewProduct
    - Encodable์ ์ฑํํ๋ DTO์๋๋ค.
    - ์ํ ๋ฑ๋ก์ ์ ๋ฌํ  ๊ฐ์ ๊ฐ์ต๋๋ค.
- ProductAddRequest
    - NetworkRequest๋ฅผ ์ฑํํ๊ณ , ์ํ ๋ฑ๋ก์ ๋ฆฌํ์คํธํ๊ธฐ์ํ ํ๋กํผํฐ๋ฅผ ๊ฐ๊ณ  ์๋ ๊ตฌ์กฐ์ฒด์๋๋ค.
- ProductEditRequest
    - NetworkRequest๋ฅผ ์ฑํํ๊ณ , ์ํ ์์ ์ ๋ฆฌํ์คํธํ๊ธฐ์ํ ํ๋กํผํฐ๋ฅผ ๊ฐ๊ณ  ์๋ ๊ตฌ์กฐ์ฒด์๋๋ค.
- URISearchRequest
    - NetworkRequest๋ฅผ ์ฑํํ๊ณ , ์ํ ์ญ์  URI๋ฅผ ๋ฆฌํ์คํธํ๊ธฐ์ํ ํ๋กํผํฐ๋ฅผ ๊ฐ๊ณ  ์๋ ๊ตฌ์กฐ์ฒด์๋๋ค.
- ProductDeleteRequest
    - NetworkRequest๋ฅผ ์ฑํํ๊ณ , ์ํ ์ญ์ ๋ฅผ ๋ฆฌํ์คํธํ๊ธฐ์ํ ํ๋กํผํฐ๋ฅผ ๊ฐ๊ณ  ์๋ ๊ตฌ์กฐ์ฒด์๋๋ค.
</details>
    
#### ๐ Step4
- UIAlertController ํ์ฉ
    - โ textFields ์ฌ์ฉํ๊ธฐ
    - โ Action Sheet ์ฌ์ฉํ๊ธฐ
    - โ preferredAction ์ฌ์ฉํ๊ธฐ
- ํ๋กํ ์ฝ ๋ฐ ๊ธฐ๋ณธ๊ตฌํ ํ์ฉํ๊ธฐ
    - โ ํ๋กํ ์ฝ๋ก ๊ณตํต๊ธฐ๋ฅ ๊ตฌํํ๊ณ  ์ฑํํ๊ธฐ
    
<details>
<summary> 
ํผ์ณ๋ณด๊ธฐ
</summary>
    
1๏ธโฃ **Controller**
- ProductManagingViewController
    - ์ํ ์์  ํ๋ฉด๊ณผ ์ํ ๋ฑ๋ก ํ๋ฉด์ ๊ณตํต ๊ธฐ๋ฅ์ ๊ตฌํํ ํ๋กํ ์ฝ์๋๋ค.
- EditProductViewController
    - ์ํ ์์ ์ ๋ณ๊ฒฝํ  ๊ฐ์ ๊ฐ์ ธ์ ํ์ํ๊ณ  ์ฌ์ฉ์์๊ฒ ์์ ๊ฐ์ ์๋ ฅ๋ฐ์ ์ฒ๋ฆฌํ๋ ๋ทฐ ์ปจํธ๋กค๋ฌ์๋๋ค.
    
2๏ธโฃ **View**
- DetailView
    - ์ํ ์์ธ ํ๋ฉด์์ ์ฌ์ฉํ๋ ๋ทฐ์๋๋ค.
    - DetailProduct๊ฐ ๊ฐ๊ณ  ์๋ ์ ๋ณด๋ฅผ ๋ํ๋ด๋ ํ์คํธ์ ์ด๋ฏธ์ง๋ฅผ ๊ทธ๋ฆฝ๋๋ค.
- DetailImageCell
    - EditProductViewController์์ ์ํ์ ์ด๋ฏธ์ง๋ฅผ ๋ด๋นํ๋ ์์๋๋ค.

3๏ธโฃ **Model**
- SendingProduct
    - ์ํ ์์ ๊ณผ ์ํ ๋ฑ๋ก์ ์ฌ์ฉํ๋ ๋ชจ๋ธ์๋๋ค.

</details>

## ๐๐ป ๊ธฐ์ ์  ๋์ 

#### โ๏ธ URLSession 
<details>
<summary>ํผ์ณ๋ณด๊ธฐ</summary>
    
- iOS ์ฑ์์ ์๋ฒ์ ํต์ ํ๊ธฐ ์ํด ์ ํ์ `URLSession`์ด๋ผ๋ API๋ฅผ ์ ๊ณตํ๊ณ  ์์ต๋๋ค. ์ ๋ชํ ๋ผ์ด๋ธ๋ฌ๋ฆฌ์ธ Alamofire, Moya ๋ฑ์ ๊ธฐ๋ฐ์ด ๋๋ API๋ก ์๋ฒ์์ ๋ฐ์ดํฐ ๊ต๋ฅ๋ฅผ ์ํด์๋ ํ์์ ์ผ๋ก ์์์ผ ํ๋ API์๋๋ค.
- `URLSession`์ HTTP๋ฅผ ํฌํจํ ๋ช ๊ฐ์ง ํ๋กํ ์ฝ์ ์ง์ํ๊ณ , ์ธ์ฆ, ์ฟ ํค ๊ด๋ฆฌ, ์บ์ ๊ด๋ฆฌ ๋ฑ์ ์ง์ํฉ๋๋ค.<br><br>
- ๐ก ์ด๋ฒ ํ๋ก์ ํธ์์๋ ์ ๊ณต๋ฐ์ ์๋ฒ์ ์๋ JSON ๋ฐ์ดํฐ๋ฅผ ๋ฐ์์ค๋๋ก ๊ตฌํํด ๋ณด์์ต๋๋ค.

</details> 

#### โ๏ธ Test Double
<details>
<summary>ํผ์ณ๋ณด๊ธฐ</summary>
    
- Test Double ํ์คํธ๋ฅผ ์งํํ๊ธฐ ์ด๋ ค์ด ๊ฒฝ์ฐ ์ด๋ฅผ ๋์ ํด ํ์คํธ๋ฅผ ์งํํ  ์ ์๋๋ก ๋ง๋ค์ด์ฃผ๋ ๊ฐ์ฒด๋ฅผ ๋งํฉ๋๋ค.
- ์ค์ ๋ก ๋คํธ์ํน์ ํ์ง ์๊ณ , ์ ์์ ์ผ๋ก fetch๊ฐ ์งํ๋๋์ง ๋ก์ง์ ํ์คํธ ํ๊ธฐ์ํด `MockURLSession`์ด๋ผ๋ test double๊ฐ์ฒด๋ฅผ ๋ง๋ค๊ณ  `MockData` ๊ฐ์ฒด๋ฅผ ๋ฐํํ๋๋ก ๋ก์ง์ ๊ตฌํํด์ผ ํ์ต๋๋ค.<br><br>
- ๐ก ์ด๋ฒ ํ๋ก์ ํธ์์๋ ์ค์  `URLSession`๊ณผ ์ด๋ฐ `MockURLSession`์ ๋ค๋ฅด๊ฒ ์๋ํด์ผ ํ๋ฏ๋ก, ํ๋กํ ์ฝ์ ํตํด ์์กด์ฑ์ ์ญ์ ์์ผ ๋คํธ์ํฌ ๋งค๋์ ๊ฐ ํ๋กํ ์ฝ์ ๋ฐ๋ผ๋ณด๊ฒ ํ์ฌ ํ์คํธ๋ฅผ ํ  ๋๋ `MockURLSession`์ ์ฃผ์์ํค๊ณ , ์ค์  ๋คํธ์ํน์ ํ  ๋๋ `URLSession`์ ์ฃผ์์ํค๋ ๋ฐฉ๋ฒ์ผ๋ก ๊ตฌํํด ๋ณด์์ต๋๋ค.

</details>

#### โ๏ธ Segmented Control
<details>
<summary>ํผ์ณ๋ณด๊ธฐ</summary>
    
- Segmented Control์ ๊ฐ๊ฐ ๋ฒํผ์ผ๋ก ๊ธฐ๋ฅํ๋ ๋ ๊ฐ ์ด์์ ์ธ๊ทธ๋จผํธ๋ก ๊ตฌ์ฑ๋ ๋ฆฌ๋์ด ์งํฉ์๋๋ค. `UISegmentedControl`๋ ์ฌ๋ฌ ์ธ๊ทธ๋จผํธ๋ก ๊ตฌ์ฑ๋ ์ํ ์ปจํธ๋กค์ด๋ฉฐ ๊ฐ ์ธ๊ทธ๋จผํธ๋ ๊ฐ๋ณ ๋ฒํผ์ผ๋ก ์๋ํฉ๋๋ค.
<br><br>
- ๐ก ์ด๋ฒ ํ๋ก์ ํธ์์๋ ์๊ตฌ์ฌํญ์ผ๋ก ์คํ๋ง์ผ ์ํ ๋ฆฌ์คํธ๋ฅผ LIST๋ชจ์๊ณผ GRID๋ชจ์ ๋๊ฐ์ง๋ก ํํํด ์ฃผ์ด์ผ ํ์ต๋๋ค. ์ด๋ฅผ ๊ฐ๊ฐ ๊ตฌํํ๊ณ  ์ธ๊ทธ๋จผํธ์ ํ ๋นํ์ฌ ์๋ก isHidden ์ํ๋ฅผ ์ ํํ๋ ๋ฐฉ์์ผ๋ก ํ๋ฉด์ ๋ณ๊ฒฝํ๋๋ก ๊ตฌํํ์์ต๋๋ค.

</details>

#### โ๏ธ UIActivityIndicatorView
<details>
<summary>ํผ์ณ๋ณด๊ธฐ</summary>
    
- `UIActivityIndicatorView`๋ ์์์ด ์งํ ์ค์์ ๋ณด์ฌ์ฃผ๋ ๋ทฐ์๋๋ค. ์ผ๋ฐ์ ์ผ๋ก ์ฌ์ฉ์์๊ฒ ๋ฐ์ดํฐ๋ฅผ ๋ถ๋ฌ์ค๊ณ  ์๋ค๋ ๊ฒ์ ์๋ ค์ฃผ๊ธฐ ์ํด ์ฌ์ฉํฉ๋๋ค.
- ์ด๋ฏธ์ง๋ฅผ ์๋ฒ์์ ๊ฐ์ ธ์ค๋ ๋ก์ง์ ํ์คํธ๋ฅผ ๊ฐ์ ธ์ค๋ ๊ฒ๊ณผ๋ ๋ค๋ฅด๊ฒ ์๊ฐ์ด ๊ฑธ๋ฆฌ๋ ์์์๋๋ค. ๋ฐ๋ผ์, ์ด๋ฏธ์ง์ ํ์ฑ์ด ๋๋  ๋ ๊น์ง ์ฌ์ฉ์๋ ์ด๋ฏธ์ง๊ฐ ์๋ ์์ ๋ณด๋ค๊ฐ ์ด๋ฏธ์ง๊ฐ ๋์ค์ ๋ํ๋๋ UI๋ฅผ ๋ณด๊ฒ ๋  ๊ฒ์๋๋ค. ์ด๋ ์ข์ ์ฌ์ฉ์ ๊ฒฝํ์ด ์๋๋ผ ํ๋จํ์ฌ ์ด๋ฏธ์ง์ ํ์ฑ์ด ๋๋  ๋ ๊น์ง ๋ก๋ฉ์ค์์ ์๋ฆฌ๋ ์๊ฐ์  ์ ๋ณด๊ฐ ํ์ํ์์ต๋๋ค.<br><br>
- ๐ก ์ด๋ฒ ํ๋ก์ ํธ์์๋ ์ด๋ฏธ์ง์ ์ ํํ ๊ฐ์ ์์น์ `UIActivityIndicatorView`๋ฅผ ์ถ๊ฐํ์ฌ ์ด๋ฏธ์ง๊ฐ ํ์ฑ๋์ด ์ด๋ฏธ์ง๋ทฐ์ ํ ๋น๋  ๋๊น์ง ๋ก๋ฉ์ค์์ ์๋ ธ์ต๋๋ค. ์ด๋ฏธ์ง๊ฐ ํ ๋น๋ ํ์๋ `UIActivityIndicatorView`์ ์ ๋๋ฉ์ด์์ ๋ฉ์ถ๊ณ  ๋ณด์ด์ง ์๊ฒ ๋ฐ๊พธ๋๋ก ๊ตฌํํ์์ต๋๋ค.

</details>

#### โ๏ธ NSCache
<details>
<summary>ํผ์ณ๋ณด๊ธฐ</summary>
    
- ์บ์ฑ์ ์ฌ์ฌ์ฉ๋  ์ ์์ ๋งํ ์์์ ํน์ ์์ญ์ ์ ์ฅํด๋๋ ๊ฒ์ ์๋ฏธํฉ๋๋ค. ์บ์ฑ๋ ๋ฐ์ดํฐ๊ฐ ์๋ค๋ฉด ์ถ๊ฐ์ ์ธ ์์์ ์๋ชจํ์ง์๊ณ  ์บ์ฑ ๋ฐ์ดํฐ๋ฅผ ๊ฐ์ ธ๋ค ์ธ ์ ์๊ธฐ ๋๋ฌธ์ ์์์ ์ ์ฝํ  ์ ์๊ณ  ์ ํ๋ฆฌ์ผ์ด์์ ์ฒ๋ฆฌ ์๋๊ฐ ํฅ์๋ฉ๋๋ค.
- NSCache๋ iOS ์ ํ๋ฆฌ์ผ์ด์์์ Memory Caching ์ ์ฃผ๋ก ์ฌ์ฉ๋๋ ํด๋์ค์๋๋ค. key-value ํํ์ ๋ฐ์ดํฐ๋ฅผ ์์๋ก ์ ์ฅํ๋ ๋ฐ ์ฌ์ฉํ  ์ ์๋ ๊ฐ๋ณ ์ปฌ๋ ์์๋๋ค. ์์์ด ๋ถ์กฑํ  ๋ ์ญ์  ๋์์ด ๋ฉ๋๋ค.
- ๋งค๋ฒ ์์ dequeueํ  ๋๋ง๋ค ์ด๋ฏธ์ง๋ฅผ ์๋ฒ์์ ๋ถ๋ฌ์ค๋ ๊ฒ์ ์์ ๋ญ๋น๊ฐ ๋๋ฌด ์ฌํ๋ค ํ๋จ๋์์ต๋๋ค. ํ๋ฒ ๋ถ๋ฌ์จ ์ด๋ฏธ์ง๋ฅผ ์บ์ฑํ์ฌ ์ด ๋ฌธ์ ๋ฅผ ํด๊ฒฐํ๊ณ ์ ํ์ต๋๋ค.<br><br>
- ๐ก ์ด๋ฒ ํ๋ก์ ํธ์์๋ `NSCache<NSString, UIImage>`ํ์์ ์ฑ๊ธํด ๊ฐ์ฒด๋ฅผ ๊ฐ๋ `ImageCacheManager` ํด๋์ค๋ฅผ ๊ตฌํํ์์ต๋๋ค. ์ด๋ฅผ ํตํด ํ ๋ฒ ์ฌ์ฉ๋ ์ด๋ฏธ์ง๋ ์บ์ฑํ์ฌ ์ฑ๋ฅ์ ํฅ์์ํฌ ์ ์๋๋ก ๊ตฌํํ์์ต๋๋ค.

</details>
    
#### โ๏ธ UIRefreshControl
<details>
<summary>ํผ์ณ๋ณด๊ธฐ</summary>
    
![](https://i.imgur.com/pmSW13Q.png)

- UIRefreshControl ๊ฐ์ฒด๋ table view์ collection view๋ฅผ ํฌํจํ ๋ชจ๋  `UIScrollView`์ ๋ถ์ผ ์ ์๋ ํ์ค ์ปจํธ๋กค์๋๋ค. ์ด ์ปจํธ๋กค์ ์คํฌ๋กค ๊ฐ๋ฅํ ๋ทฐ์ ์ถ๊ฐํ๋ฉด ์ฌ์ฉ์๋ ํ์ค์ ์ธ ๋ฐฉ๋ฒ์ผ๋ก ์ปจํ์ธ ๋ฅผ ์๋ก๊ณ ์นจํ  ์ ์์ต๋๋ค.
- ์ฌ์ฉ์๋ ์๋๋ก ์คํฌ๋กค์ ์๋๋ก ๋น๊ธฐ๋ฉด ๋ฆฌํ๋ ์ ์ธ๋์ผ์ดํฐ๋ฅผ ์ง๊ด์ ์ผ๋ก ํ์ธํ  ์ ์์ผ๋ฉฐ, ๋ฆฌํ๋ ์ฑ ๋ก์ง์ด ๋๋๋ฉด ์ธ๋์ผ์ดํฐ๊ฐ ์ฌ๋ผ์ ธ ์์์ด ๋๋ฌ์์ ์ ์ ์์ต๋๋ค.<br><br>
- ๐ก ์ด๋ฒ ํ๋ก์ ํธ์์๋ ์คํฌ๋กค์ ์๋๋ก ๋น๊ธฐ๋ฉด ์ํ๋ชฉ๋ก์ ์๋ฐ์ดํธ ํ์ฌ ์๋ก ๋ฑ๋ก๋ ์ํ์ ์ํ๋ ๋์ ๋ฐ๋ก๋ฐ๋ก ํ์ธํ  ์ ์๋๋ก ๊ตฌํํ์์ต๋๋ค.
- ๋ํ, ์๋ฐ์ดํธ๊ฐ ์๋ฃ๋๋ ์์ ๋ณด๋ค 1์ด์ ์ฌ์  ์๊ฐ์ ๋ ์ค์ ์ฌ์ฉ์์๊ฒ ๋คํธ์ํน์ด ์งํ์ค์ด๋ผ๋ ์ ๋ณด๋ฅผ ํ์คํ๊ฒ ์ ๋ฌํ๋๋ก ๊ตฌํํ์์ต๋๋ค.
    
</details>

#### โ๏ธ UICollectionViewDiffableDataSource
<details>
<summary>ํผ์ณ๋ณด๊ธฐ</summary>
    
- iOS13๋ถํฐ ์ฌ์ฉ ๊ฐ๋ฅํ Generic Class๋ก, tableView๋ collectionView๋ฅผ ์ด์  ๋ฐฉ์๋ณด๋ค ๋น๊ต์  ๋จ์ํ๊ฒ ์๋ฐ์ดํธ๊ฐ ๊ฐ๋ฅํด์ง๋๋ค. ์ด์  ํ์ด๋ธ๊ณผ ๋ฌ๋ผ์ง ๋ถ๋ถ์ ์๋์ผ๋ก ์์์ฐจ๋ฆฌ๊ณ , ์๋ก์ด ๋ถ๋ถ๋ง ๋ค์ ๊ทธ๋ฆฌ๊ธฐ ๋๋ฌธ์๋๋ค.
- ์ด Diffable์ ์ฌ์ฉํ์ฌ ์ป๊ฒ ๋๋ ํจ๊ณผ์ ์ฅ์ ์:
    1. ์ถ๊ฐ์ ์ธ ์ฝ๋์์ ์์ด๋, ์ ๋๋ฉ์ด์ ์ ์ฉ์ด ๊ฐ๋ฅํฉ๋๋ค.
    2. ๊ฐ์ ๋ Data Source ๋งค์ปค๋์ฆ์ ์๋ฒฝํ๊ฒ ๋๊ธฐ์ ์ธ ๋ฒ๊ทธ๋, ์์ธ, ์ถฉ๋ ์ํฉ๋ค์ ํผํ  ์ ์๊ฒ ํด์ค๋๋ค.
    3. UI ๋ฐ์ดํฐ์ ๋๊ธฐํ ๋ถ๋ถ ๋์  ์ฑ์ ๋์ ์ธ ๋ฐ์ดํฐ์ ๋ด์ฉ์ ์ง์คํ  ์ ์๊ฒ ํด์ค๋๋ค.
    4. identifier์ snapshot์ ์ฌ์ฉํ๋ ๊ฐ์ํ ๋ Data ๋ชจ๋ธ์ ์ ์ ํ๊ณ , ์ด๋ฅผ ์ด์ฉํ์ฌ UI๋ฅผ ์๋ฐ์ดํธ ํฉ๋๋ค.<br><br>
- ๐ก ์ด๋ฒ ํ๋ก์ ํธ์์๋ ์ํ๋ฑ๋ก ๋ฐ ์์  ํ๋ฉด์์ ์ํ์ ์ฌ์ง์ ์ถ๊ฐํ  ๋ ๋ง๋ค ์์ฐ์ค๋ฝ๊ฒ ์์ด ์ถ๊ฐ๋๊ณ , ๊ฐ๋ก๋ก ์คํฌ๋กค๋๋๋ก ๊ตฌํํ์์ต๋๋ค.
    
</details>

#### โ๏ธ UIAlertController
<details>
<summary>ํผ์ณ๋ณด๊ธฐ</summary>
    
- ์ผ๋ฟ ๋ฉ์์ง๋ฅผ ํ์ํ๋ ๊ฐ์ฒด๋ก preferredStyle์ ๋ฐ๋ผ alert๊ณผ actionSheet๊ฐ ์์ต๋๋ค.
- ์ฌ์ฉ์์๊ฒ ๋ฉ์์ง๋ฅผ ํ์ํ๋ ๊ฒ ์ธ์๋ ์ผ๋ฟ ์ปจํธ๋กค๋ฌ์ ์ก์์ ์ฐ๊ฒฐํ์ฌ ์ฌ๋๋ค์ด ์๋ตํ  ์ ์๋ ๋ฐฉ๋ฒ์ ์ ๊ณตํ  ์ ์์ต๋๋ค.
- ์ฌ์ฉ์๊ฐ ํด๋น ์ก์์ ํญํ๋ฉด ๊ฒฝ๊ณ  ์ปจํธ๋กค๋ฌ๋ ์์ ๊ฐ์ฒด๋ฅผ ๋ง๋ค ๋ ์ ๊ณตํ ์ฝ๋ ๋ธ๋ก์ ์คํํฉ๋๋ค.
- ๋ํ, textFields๋ฅผ ํ๋กํผํฐ๋ก ๊ฐ์ง๊ณ  ์์ด ์ด๋ฅผ ์ด์ฉํ๋ฉด ์ฌ์ฉ์์๊ฒ ๋ฉ์์ง๋ฅผ ์ ๊ณตํจ๊ณผ ๋์์, ํ์ํ ์ ๋ณด๋ฅผ ์ ๊ณต๋ฐ์ ์ฒ๋ฆฌํ  ์ ์์ต๋๋ค.
- ๐ก ์ด๋ฒ ํ๋ก์ ํธ์์๋ ์ํ ์์ธํ๋ฉด์์ ์ก์์ํธ๋ฅผ ํตํด ์ํ ์์ ๊ณผ ์ญ์ ์ ๋ํ ์ก์์ ์ ๊ณตํ๊ณ , ์ํ ๋ฑ๋ก ํ๋ฉด ๋ฑ์์ ์ผ๋ฟ์ ํตํด ์ฌ์ฉ์์๊ฒ ๋ฉ์์ง๋ฅผ ํ์ํ๋ฉฐ, ์ํ์ ์ญ์ ํ๋ ๊ฒฝ์ฐ ์ฌ์ฉ์์๊ฒ ๋น๋ฐ๋ฒํธ๋ฅผ ์ ๋ฌ๋ฐ์ ์ผ์นํ๋ ๊ฒฝ์ฐ์๋ง ์ญ์ ํ๋๋ก ๊ตฌํํด ๋ณด์์ต๋๋ค.
    
</details>
    
### collectionView์ Paging
<details>
<summary>ํผ์ณ๋ณด๊ธฐ</summary>
   
- scrollView์์ paging ๊ธฐ๋ฅ์ ํ์ฑํํ๋ฉด scrollView๋ ์ฌ์ฉ์๊ฐ ์คํฌ๋กคํ  ๋ scrollView์ ๊ฒฝ๊ณ์์ ์ ์งํฉ๋๋ค.
- scrollView๋ฅผ ์์๋ฐ๋ collectionView์ ๊ฒฝ์ฐ์๋ paging ๊ธฐ๋ฅ์ ์ฌ์ฉํ  ์ ์๊ณ , ์, ๊ทธ๋ฃน, ์น์ ๋ฑ์ ์ง์ ํ  ์ ์์ต๋๋ค.
- iOS 13๋ถํฐ ์ฌ์ฉ ๊ฐ๋ฅํ NSCollectionLayoutSection์ ๊ฒฝ์ฐ orthogonalScrollingBehavior ํ๋กํผํฐ๋ฅผ groupPagingCentered ๋ฑ์ผ๋ก ์ค์ ํ๋ฉด ์๋์ผ๋ก paging์ ๊ณ์ฐํด์ค๋๋ค.
- ์ํ ์์ธ ํ์ด์ง์์์ ์ด๋ฏธ์ง๋ ๋์ฑ ์ฉ๋์ด ํฐ ์๋ณธ ์ด๋ฏธ์ง์๋๋ค.
- ์ด ์ด๋ฏธ์ง๋ค์ ํ๋์ฉ ์ ํ์ธํ  ์ ์๋๋ก ํ๋ฉด์ ๊ฐ๋ ๋ฉ์ฐ๋ ํฌ๊ธฐ๋ก ์ด๋ฏธ์ง๋ฅผ ํ์ํฉ๋๋ค.
- ๋ํ ์ด๋ฏธ์ง๋ณ๋ก ์ฌ์ง์ ๋ฒํธ๊ฐ ๋ ์ด๋ธ๋ก ํ์๋ฉ๋๋ค.
- ๐ก ์ด๋ฒ ํ๋ก์ ํธ์์๋ ์ํ ์์ธ ํ์ด์ง์ ์ด๋ฏธ์ง๋ฅผ ํ๋์ฉ ์ ํ์ธํ  ์ ์๋๋ก ๋ ๋ชํํ UI/UX๋ฅผ ์ํด Paging ๊ธฐ๋ฅ์ ์ฌ์ฉํ์์ต๋๋ค.
        
</details>

## ๐ ํธ๋ฌ๋ธ ์ํ ๋ฐ ๊ณ ๋ฏผ
    
#### ๐ ํ์คํธ์ฉ JSON ํ์ผ๊ณผ ์๋ฒ API ๋ฌธ์
    
<details>
<summary> 
ํผ์ณ๋ณด๊ธฐ
</summary>

**๋ฌธ์  ๐ป**
- ์ด๋ฒ ํ๋ก์ ํธ ์๋ดํ์ด์ง์์ ์ ๊ณตํ๋ ํ์คํธ์ฉ JSON ํ์ผ๊ณผ ์์ผ๋ก ์์์ ์งํํ  API์ JSON์ด ์๋ก CodingKey๋ value์ ํ์์ด ๋ฌ๋์ต๋๋ค. 
```json
// ํ์คํธ์ฉ JSON ํ์ผ
{
  "page_no": 1,
  "items_per_page": 20,
  "total_count": 10,
  "offset": 0,
  "limit": 20,
    ...
}
```
```json
// ์๋ฒ API ๋ฌธ์
{
  "pageNo": 1,
  "itemsPerPage": 20,
  "totalCount": 10,
  "offset": 0,
  "limit": 20,
    ...
}
```
- ์ฐ์  ํ์คํธ์ฉ ํ์ผ์ ๋ง๊ฒ DTO๋ฅผ ๊ตฌํํ์๋๋ฐ, ์ค์  API Network๋ฅผ ์งํํด๋ณด๋ฉด์ ์๋ก ๋ค๋ฅด๋ค๋ ๊ฒ์ ์๊ฒ ๋์์ต๋๋ค. 

**ํด๊ฒฐ ๐ซ**
- ํ์คํธ์ ์ทจ์ง๊ฐ ๋คํธ์ํฌ๊ฐ ์๋ ์ํฉ์์๋ ์ ์์ ์ผ๋ก ๋์ํ๋์ง๋ฅผ ๊ฒ์ฆํ๋ ๊ฒ์ด๊ธฐ ๋๋ฌธ์ ์๋ฒ API ๋ฌธ์์ ๋ฐ์ดํฐ ํ์์ ๋ง์ถ๋ ๊ฒ์ด ์ ์ ํ๋ค๊ณ  ์๊ฐํด ํ์คํธ์ฉ JSON ํ์ผ์ ์๋ฒ API ๋ฌธ์์ ๋ฐ์ดํฐ ํ์์ ๋ง๊ฒ ์์ ํ์์ต๋๋ค. 

</details>

#### ๐ Deprecated Initializer

<details>
<summary> 
ํผ์ณ๋ณด๊ธฐ
</summary>

**๋ฌธ์  ๐ป**
- ํ์คํธ ๋๋ธ์ ์ํด URLSessionProtocol์ ์ ์ํ์์ต๋๋ค.
```swift
protocol URLSessionProtocol {
    func dataTask(with url: URL,
                  completionHandler: @escaping DataTaskCompletionHandler
    ) -> URLSessionDataTask
}
```
- ์ด ๋ `URLSessionDataTask`ํ์๋ Mock๋ฐ์ดํฐ๋ก ๋ง๋ค์ด ์ฃผ์๋๋ฐ, ์ด ํ์์ ์ด๊ธฐํ ๊ตฌ๋ฌธ์ด iOS13๋ฒ์  ๋ถํฐ ๋ ์ด์ ์ฌ์ฉ๋์ง ์๋(deprecated) ๋ก์ง์ด์ด์ ํ์ฌ ๋์์ ์ํํ์ง๋ง ์ ์ ํ์ง ์์ ๋ฐฉ๋ฒ์ด๋ผ๊ณ  ์๊ฐํ์ต๋๋ค.
![](https://i.imgur.com/0ipjyRN.png)
![](https://i.imgur.com/Dzncleq.png)

**ํด๊ฒฐ ๐ซ**
- `URLSessionDataTask`๋ฅผ ์ง์  ์ฌ์ฉํ์ง ์๊ณ  URLSessionProtocol๊ณผ ๋ง์ฐฌ๊ฐ์ง๋ก ์์กด์ฑ์ ์ญ์ ์์ผ URLSessionProtocol์ด ํ๋กํ ์ฝ์ ๋ฐ๋ผ๋ณด๊ฒ ๊ตฌํํ์์ต๋๋ค.
```swift
protocol URLSessionProtocol {
    func dataTask(with url: URL,
                  completionHandler: @escaping DataTaskCompletionHandler
    ) -> URLSessionDataTaskProtocol
}

protocol URLSessionDataTaskProtocol {
    func resume()
}
```

</details>

#### ๐ญ ์ฌ์ฌ์ฉ์ด ๊ฐ๋ฅํ Request๊ฐ์ฒด ๊ตฌํํ๊ธฐ
    
<details>
<summary> 
ํผ์ณ๋ณด๊ธฐ
</summary>
    
```swift
protocol NetworkRequest {
    var httpMethod: HttpMethod { get }
    var urlHost: String { get }
    var urlPath: String { get }
    var queryParameters: [String: String] { get }
}

extension NetworkRequest {
    var url: URL? {
        if queryParameters.isEmpty {
            return URL(string: urlHost + urlPath)
        }
        var urlComponents = URLComponents(string: urlHost + urlPath)
        let queryItems = queryParameters.map { URLQueryItem(name: $0, value: $1) }
        urlComponents?.queryItems = queryItems
        
        return urlComponents?.url
    }
}

```
**๊ณ ๋ฏผ ๐ค**
- ์ด๋ฒ ํ๋ก์ ํธ์์ ๋คํธ์ํน์ ์์๊ฐ ์ด 3๊ฐ์ง ์์ต๋๋ค.
- ๊ทธ๋ฆฌ๊ณ  ์ค์  ์คํ๋ง์ผ ์๋ฒ์์๋ GET๋ฉ์๋ ๋ง๊ณ ๋ POST, PATCH, DEL ๋ฑ์ httpMethod๋ฅผ ์ฌ์ฉํ  ์ ์์์ต๋๋ค.
- ์ด์ ๊ฐ๊ฐ์ ๋ฆฌํ์คํธ๋ง๋ค URL์ฃผ์๊ฐ ๋ฌ๋ผ์ก์๊ณ , ์ด๋ฅผ String์ผ๋ก ์จ์ฃผ๋๊ฑด ์ฝ๋์ ์ฌ์ฌ์ฉ์ด ๋ง๊ณ , ํ์ฅ์ฑ์๋ ๋ฌธ์ ๊ฐ ์์ด๋ณด์ธ๋ค ํ๋จํ์์ต๋๋ค.
- ๊ทธ๋์ `NetworkRequest` ํ๋กํ ์ฝ์ ๋ง๋ค๊ณ , ๊ฐ ๋คํธ์ํน ์์๋ฅผ ๊ฐ์ฒดํํ์ฌ ์ด๋ฅผ ์ฑํํ๋๋ก ํ์์ต๋๋ค.
- ์ด๋ก์จ URL์ String์ผ๋ก ์ง์  ์์ฑํ  ํ์๊ฐ ์์ด ํ๋กํ ์ฝ์ ์ฑํํ๊ณ  ๊ทธ ํ๋กํ ์ฝ์ ๊ฐ์์ ์ญํ ์ ๋ง๊ฒ ๊ตฌํ๋ง ํด์ฃผ๋ฉด ์์์ URL๊ณผ Request๋ฅผ ๋ง๋ค๊ฒ ๋์์ต๋๋ค.

</details>
    
#### ๐ญ BoringSSL
    
<details>
<summary> 
ํผ์ณ๋ณด๊ธฐ
</summary>

**๊ณ ๋ฏผ ๐ค**
- Step 1-2๋ฅผ ์งํํ๋ฉด์ ์๋ฒ์ ์ค์ ๋ก ๋ฐ์ดํฐ๋ฅผ ์ฃผ๊ณ  ๋ฐ์ ๋, `boringssl_metrics_log_metric_block_invoke(153)` ๋ผ๋ ๋ฉ์์ง๊ฐ ์ฝ์์ ๋จ๊ฒ ๋์์ต๋๋ค. 
- [boringssl_metrics_log_metric_block_invoke(151) Failed to log metrics](https://github.com/firebase/firebase-ios-sdk/issues/9262)์ ๋ด์ฉ ๋ฐ ์ฌ๋ฌ ๊ฒ์๊ธ๋ค์ ์ฐพ์๋ณธ ๊ฒฐ๊ณผ ๊ธฐ๋ฅ์๋ ๋ฌธ์ ๊ฐ ์๊ณ , ์ฝ์์ ๋ํ๋๊ธฐ๋ง ํ๋ ๋ฉ์์ง๋ก ํ์ํ์ต๋๋ค. 
- ์คํค๋ง์์ OS_ACTIVITY_MODE๋ฅผ disable๋ก ๋ฐ๊ฟ์ฃผ๋ฉด ์ด ์๋ฌ ๋ฉ์ธ์ง๊ฐ ์ฝ์์์ ๋ํ๋์ง ์์ง๋ง, `NSLog`๋ ์ฌ๋ผ์ง๋ ๋ฌธ์ ๊ฐ ์์ด์ ์ด ๋ฐฉ๋ฒ์ ์ ์ ํ ๋ฐฉ๋ฒ์ด ์๋๋ผ ํ๋จํ์์ต๋๋ค.
- ๋ ๋ค๋ฅธ ๋ฐฉ๋ฒ์ผ๋ก๋ `xcrun simctl spawn booted log config --subsystem com.apple.network --category boringssl --mode level:off` ์ฒ๋ผ Xcode ์ค์ ์ ๊ฑด๋๋ฆฌ๋ ๋ฐฉ๋ฒ๋ ์์๋๋ฐ, ์ด๋ Xcode์ ์ค์ ์ ๊ฑด๋๋ฆฌ๋ ๊ฒ์ด๊ณ , ์ด๋ค ์ฌ์ด๋ ์ดํํธ๊ฐ ๋ฐ์ํ ์ง ๋ชฐ๋ผ, ์ ์ฉํ๊ธฐ์ ์ ์ ํ์ง ์๋ค ํ๋จํ์ฌ ์ ์ฉํ์ง ์์์ต๋๋ค.

</details>

#### ๐ ํฌ๋ชํ ๋ค๋น๊ฒ์ด์ ๋ฐ ๋ฌธ์  ํด๊ฒฐํ๊ธฐ

<details>
<summary> 
ํผ์ณ๋ณด๊ธฐ
</summary>

**๋ฌธ์  ๐ป**
- ์ฑ ๊ตฌ๋์ ๋ค๋น๊ฒ์ด์ ๋ฐ๊ฐ ํฌ๋ชํด์ ธ์ ๋ค๋น๊ฒ์ด์ ๋ฐ ์์ดํ๋ค์ด ๋ฅ๋ฅ ๋ ๋ค๋๋ ๋ชจ์ต์ด ๋์ด๋ฒ๋ ธ์ต๋๋ค.
![](https://i.imgur.com/ajEo04E.png)
- ์ด๋ iOS๊ฐ 15๋ฒ์ ์ผ๋ก ์๋ฐ์ดํธ ๋ ํ ๋ค๋น๊ฒ์ด์ ๋ฐ๊ฐ ํ์ฅ๋๋ฉด์ ์๊ธด ๋ฌธ์ ์์ต๋๋ค. ์๋ฎฌ๋ ์ดํฐ์ iOS๋ฒ์ ์ 15 ์๊ณ , ์๋ฎฌ๋ ์ดํฐ์์ ๋ค๋น๊ฒ์ด์ ๋ฐ๊ฐ ํฌ๋ชํด ์ง ๊ฒ์๋๋ค.

**ํด๊ฒฐ ๐ซ**
- ์ ํฌ๊ฐ ์ํ๋ ๋ฐฉํฅ์ฑ์ ๋ค๋น๊ฒ์ด์ ๋ฐ๊ฐ ํญ์ ๋ถํฌ๋ชํ๊ฒ ์๋ฆฌ๋ฅผ ์ก๋ ๊ฒ์ด๊ธฐ ๋๋ฌธ์ UINavigationBarAppearance์ configureWithDefaultBackground() ์ธ์คํด์ค ๋ฉ์๋๋ฅผ ์ฌ์ฉํด์ ํญ์ ๋ถํฌ๋ชํ๊ฒ ๋์ค๋๋ก ์ฒ๋ฆฌํ์์ต๋๋ค.
```swift
func application(_ application: UIApplication, didFinishLaunchingWithOptions launchOptions: [UIApplication.LaunchOptionsKey: Any]?) -> Bool {
        let navigationBarAppearance = UINavigationBarAppearance()
        navigationBarAppearance.configureWithDefaultBackground()
        
        UINavigationBar.appearance().standardAppearance = navigationBarAppearance
        UINavigationBar.appearance().compactAppearance = navigationBarAppearance
        UINavigationBar.appearance().scrollEdgeAppearance = navigationBarAppearance
        return true
    }
```
![](https://i.imgur.com/20jVluj.png)
    
</details>

#### ๐ ๋น๋๊ธฐ๋ก ์ธํ race-condition๋ฐ์ ๋ฌธ์  ํด๊ฒฐ

<details>
<summary> 
ํผ์ณ๋ณด๊ธฐ
</summary>

**๋ฌธ์  ๐ป**
- ์ด๋ฏธ์ง๋ฅผ ์๋ฒ์์ ๊ฐ์ ธ์ค๋ ๋ก์ง์ ๊ฒฝ์ฐ, ์ด๋ฏธ์ง์ ํฌ๊ธฐ๊ฐ ์ปค ๋ถ๋ฌ์ค๋ ์์์ ๋ฉ์ธ ์ค๋ ๋์์ ์งํํ๋ฉด ์คํฌ๋กค์ ๋ด๋ฆด ๋ ๋ง๋ค ํ๋ฉด์ด ๋ฒ๋ฒ์ด๊ฒ ๋์ด ์พ์ ํ ์ฌ์ฉ์ ๊ฒฝํ์ ์ ๊ณตํ์ง ๋ชปํ๊ฒ ๋ฉ๋๋ค.
- ๋ฐ๋ผ์ ์ด ๋ก์ง์ ๋ฉ์ธ ์ค๋ ๋๊ฐ ์๋ ๋ค๋ฅธ ์ค๋ ๋์์ ์งํํ๋๋ก ํ์ฌ ๋ฉ์ธ ์ค๋ ๋๋ ๋ฐ์์จ ์ด๋ฏธ์ง๋ฅผ ๋์ฐ๊ธฐ๋ง ํ๋๋ก ๋ก์ง์ ์ง๋ณด์์ต๋๋ค.
๋ฌธ์ ๋ ์ด ์์์ ๋น๋๊ธฐ์ ์ผ๋ก ์งํํ๋ค๋ณด๋, ์ด๋ฏธ์ง๋ฅผ ๋ถ๋ฌ์ค๊ธฐ ์ํ thumbnail์ ์ ๊ทผํ๋ ๊ณผ์ ์์ race-condition์ด ๋ฐ์ํ๋ ๊ฒ์๋๋ค. ๋๋ฌธ์ ์คํฌ๋กค์ ๋น ๋ฅด๊ฒ ๋ด๋ฆด ์๋ก ์ด๋ฏธ์ง๊ฐ ๊ณ์ ๋ฐ๋๋ ์ํ๊ฐ ๋์์ต๋๋ค.

![](https://i.imgur.com/RzInO7A.gif)

**ํด๊ฒฐ ๐ซ**
- ์ด๋ฅผ ํด๊ฒฐํ๊ธฐ ์ํด ์ด๋ฏธ์ง๋ฅผ ๋ถ๋ฌ์ค๊ธฐ ์ ์ ์์ด ๊ฐ์ง๊ณ  ์๋ product์ ๋์คํจ์น ํ๋ก ์์์ ๋๊ธธ ๋ ์บก์ณํ product๊ฐ ์ผ์นํ๋์ง ํ์ธํ๋ ๋ก์ง์ ์ถ๊ฐํ์๊ณ , product๊ฐ ๋น๊ต ๊ฐ๋ฅํ ์ํ๊ฐ ๋  ์ ์๋๋ก Hashable์ ์ฑํํ๋๋ก ์ฒ๋ฆฌํ์์ต๋๋ค.
```swift
DispatchQueue.main.async { [weak self] in
    if product == self?.product {
        self?.productImage.image = image
        self?.loadingView.stopAnimating()
        self?.loadingView.isHidden = true
        self?.productImage.isHidden = false
    }
}
```
![](https://i.imgur.com/DeWDRlh.gif)
    
</details>

#### ๐ญ ์ฝ๋๋ก๋ง ํ๋ฉด ๊ตฌํํ๊ธฐ

<details>
<summary> 
ํผ์ณ๋ณด๊ธฐ
</summary>

**๊ณ ๋ฏผ ๐ค**
- ์ด๋ฒ ํ๋ก์ ํธ๋ ์ ๋ ์คํ ๋ฆฌ๋ณด๋๋ก ๊ตฌํํ๊ธฐ๊ฐ ๋ ์ฌ์ ์ ๊ฒ ๊ฐ์ต๋๋ค.
- ํ์ง๋ง ์์ชฝ ๋ชจ๋ ํ  ์ค ์์์ผํ๊ธฐ ๋๋ฌธ์ ์ด๋ฒ ํ๋ก์ ํธ์์๋ ์ฝ๋๋ก๋ง ํ๋ฉด์ ๊ตฌํํ๋ ๊ฒ์ ๋ชฉํ๋ก ํ์ต๋๋ค.
- ์ด ๊ณผ์ ์์ ์คํ ๋ฆฌ๋ณด๋ ์ญ์  ๋ฐ ์ด๊ธฐ ์ค์ ์ผ๋ก ํ์ํ ๋ถ๋ถ๋ค์ AppDelegate ๋ฐ SceneDelegate์ ์์ฑํ์ฌ ์งํํ์ต๋๋ค.
```swift
func scene(_ scene: UIScene, willConnectTo session: UISceneSession, options connectionOptions: UIScene.ConnectionOptions) {
    guard let scene = scene as? UIWindowScene else { return }
    let rootViewController = ProductsViewController()
    let navigationController = UINavigationController(rootViewController: rootViewController)

    window = UIWindow(frame: scene.coordinateSpace.bounds)
    window?.windowScene = scene
    window?.rootViewController = navigationController
    window?.makeKeyAndVisible()
}
```

</details>

#### ๐ญ ์์ ํ Collection ์ฌ์ฉ์ ์ํ extension

<details>
<summary> 
ํผ์ณ๋ณด๊ธฐ
</summary>

**๊ณ ๋ฏผ ๐ค**
- ์ ํฌ๋ API๋ฅผ ํตํด ๋ฐ์ดํฐ๋ฅผ ์์ฒญํ  ๋ ํ ๋ฒ์ 20๊ฐ์ฉ ์์ฒญ์ ํ๊ณ  ์์ต๋๋ค.
- ๋์ด์ ๋ถ๋ฌ์ฌ ๋ฐ์ดํฐ๊ฐ ์๋ ๋ง์ง๋ง์ ๊ฐ์๋ 20๊ฐ๋ณด๋ค ์ ๊ฒ ์๋ต์ด ์ฌ ์ ์๊ธฐ ๋๋ฌธ์ ์๋ชป๋ ์ธ๋ฑ์ค์ ์ ๊ทผํ  ๊ฐ๋ฅ์ฑ์ด ์์์ต๋๋ค.
- ์ด์ ๋ํ ๋ฐํ๊ฐ์ ์ต์๋์ด ์๋ ํ์์ด๊ธฐ ๋๋ฌธ์ ์ด๋ฅผ nil์ธ์ง ํ์ธํ๋ ๊ณผ์ ์ ๋ง๋๋ ๊ฒ ๋ณด๋ค๋ subscript ๋ฌธ๋ฒ์ผ๋ก ์ ๊ทผํ  ๋ ์ต์๋ ๊ฐ์ ๋ฐํํ๊ฒ ์ฒ๋ฆฌํ๋ ๊ฒ์ด ๋ ์ ์ ํ๋ค๊ณ  ์๊ฐํ์ต๋๋ค.
- subscript ๋ฌธ๋ฒ์ ๋ํ ๋ฉ์๋ ์ถ๊ฐ๋ก ์์ ํ๊ฒ ๊ฐ์ ์ ๊ทผํ๋๋ก ํ์์ต๋๋ค.
```swift
extension Collection {
    subscript(valid index: Index) -> Element? {
        return indices.contains(index) ? self[index] : nil
    }
}
```

```swift
func collectionView(_ collectionView: UICollectionView, numberOfItemsInSection section:
Int) -> Int {
    return productLists[valid: section]?.pages.count ?? 0
}
```

</details>
    

#### ๐ multipart/form-data httpBody
    
<details>
<summary> 
ํผ์ณ๋ณด๊ธฐ
</summary>

**๋ฌธ์  ๐ป**
```http
// Header
identifier: "test"
Content-Type: "multipart/form-data; boundary=----D29749DE-06BB-43ED-B94A-D9F2550C9496"

// Body
----A5A44C23-8AE2-44FE-9CEA-019BAD96EA2D
Content-Disposition: form-data; name="params"
Content-Type: application/json

{"secret":"test","discounted_price":100,"price":10000,"stock":10,"description":"์๋ก์ด ์ํ์๋๋ค.","currency":"KRW","name":"์๋ก์ด ์ํ"}
----A5A44C23-8AE2-44FE-9CEA-019BAD96EA2D
Content-Disposition: form-data; name="images"; filename="image.jpeg"
Content-Type: image/jpeg

image Data
----A5A44C23-8AE2-44FE-9CEA-019BAD96EA2D--    
```
- multipart/form-data์ Body๋ฅผ ๋ง๋ค์ด POST ์์ฒญ์ ๋ณด๋ด๋ ๊ณผ์ ์์, ๊ณ์ํด์ `statusCode - 400` ์๋ฌ๊ฐ ๋ํ๋๋ ๋ฌธ์ ๊ฐ ์์์ต๋๋ค.
- ์์ ๊ฐ์ ๋ฐฉ๋ฒ์ผ๋ก Header์ Body๋ฅผ ๊ตฌ์ฑํ์ฌ ์๋ํด ๋ณด์์ง๋ง `MissingServletRequestPartException`๋ผ๋ ๋ฉ์ธ์ง์ ํจ๊ป,  `statusCode - 400` ์๋ฌ๊ฐ ๋ํ๋ฌ์ต๋๋ค.
    
**ํด๊ฒฐ ๐ซ**
```http
// Header
identifier: "test"
Content-Type: "multipart/form-data; boundary=----D29749DE-06BB-43ED-B94A-D9F2550C9496"

// Body
------A5A44C23-8AE2-44FE-9CEA-019BAD96EA2D
Content-Disposition: form-data; name="params"
Content-Type: application/json

{"secret":"test","discounted_price":100,"price":10000,"stock":10,"description":"์๋ก์ด ์ํ์๋๋ค.","currency":"KRW","name":"์๋ก์ด ์ํ"}
------A5A44C23-8AE2-44FE-9CEA-019BAD96EA2D
Content-Disposition: form-data; name="images"; filename="image.jpeg"
Content-Type: image/jpeg

image Data
------A5A44C23-8AE2-44FE-9CEA-019BAD96EA2D--    
```
- ๋ณดํต ์ด๋ฐ 400 ์๋ฌ์ ๊ฒฝ์ฐ multipart/form-data๊ฐ ์๊ตฌํ๋ ํผ์ผ๋ก ๋ฐ์ดํฐ๋ฅผ ์์ฑํ์ง ์์ ๋ ์๊ธฐ๋ ์๋ฌ์๋๋ค.
- ์ธ๋ป ๋ณด๋ฉด ์ ์ง์ผ์ ์์ฑํ ๊ฒ ๊ฐ์ง๋ง, ์์ธํ๊ฒ ๋ณด๋ ๋ฐ์ด๋๋ฆฌ ์์ `--`๋ฅผ ์ถ๊ฐ์ ์ผ๋ก ์๋ ฅํ์ง ์์์ ๋ฐ์ํ ๋ฌธ์ ์์ต๋๋ค.
- ๋ฐ์ด๋๋ฆฌ๋ฅผ ์ ์ธํ๋ ๋ถ๋ถ๊ณผ ๋ค๋ฅด๊ฒ ๋ฐ์ด๋๋ฆฌ๋ฅผ ์ฌ์ฉํ๋ ๋ถ๋ถ(์ค์  ๋ฉํฐํํธ๋ฅผ ๊ตฌ๋ถํ๋ ๋ถ๋ถ)์์๋ ์ถ๊ฐ ์ ๋์ฌ๋ก `--`์ ๋ฐ๋์ ๋ถ์ฌ์ฃผ์ด์ผ ํฉ๋๋ค.
- ์ด๋ฅผ ์ ์ฉํ์ฌ ๋ฌธ์ ๋ฅผ ํด๊ฒฐํ์์ต๋๋ค.

</details>

#### ๐ ๋ชจ๋ ์ปฌ๋ ์๋ทฐ ๊ฐ๋ก ์คํฌ๋กค
    
<details>
<summary> 
ํผ์ณ๋ณด๊ธฐ
</summary>

**๋ฌธ์  ๐ป**
- ๋ชจ๋ ์ปฌ๋ ์๋ทฐ๋ฅผ ํตํด ์ํ ๋ฑ๋ก/์์  ํ์ด์ง์ ์ด๋ฏธ์ง ๋ชฉ๋ก ๊ฐ๋ก ์คํฌ๋กค์ ๊ตฌํํ์์ต๋๋ค.
- ํ์ง๋ง ์ปฌ๋ ์๋ทฐ ์์ฒด์ ์คํฌ๋กค๋๋ฌธ์ ์ข์ฐ๋ง์ด ์๋ ์์๋๋ก๋ ์คํฌ๋กค ๊ธฐ๋ฅ์ด ์ด์์์์ต๋๋ค.
![](https://i.imgur.com/r5phSYP.gif)

**ํด๊ฒฐ ๐ซ**
- ์ด๋ฅผ ํด๊ฒฐํ๊ธฐ ์ํด `configureCollectionView()` ๋ฉ์๋๋ฅผ ํธ์ถํ  ๋ ์ปฌ๋ ์๋ทฐ์ `isScrollEnabled` ํ๋กํผํฐ๋ฅผ false๋ก ๋ณ๊ฒฝํด์ฃผ์์ต๋๋ค.
![](https://i.imgur.com/5oUHwyj.gif)
```swift
private func configureCollectionView() {
    imageCollectionView.isScrollEnabled = false
```

</details>
    
#### ๐ญ ํ๋์ CollectionView ์ฌ์ฉํ๊ธฐ

<details>
<summary> 
ํผ์ณ๋ณด๊ธฐ
</summary>

**๊ณ ๋ฏผ ๐ค**
- ๋ ๊ฐ์ collectionView๋ฅผ hide/unhideํ๋ฉด์ ํ๋ฉด์ ์ ํํ๋ ๋ฐฉํฅ์ผ๋ก ํ๋ก์ ํธ๋ฅผ ์งํํ์ต๋๋ค.
- ํ์ง๋ง ์ปฌ๋ ์๋ทฐ์ ๋ ์ด์์๋ง์ ๊ต์ฒดํ๋ ๊ฒ์ด ๋์ฑ ์์์ ํ์ฉ์ ์ธ ์ธก๋ฉด์์ ์ข์ ๊ฒ์ด๋ผ๊ณ  ์๊ฐํ์ต๋๋ค.
- ํ๋์ ์ปฌ๋ ์๋ทฐ๋ก ํ์ฉํ  ์ ์๋๋ก ์ ์ฝ์ฌํญ ๋ฑ์ ์ ๋ฆฌํ๊ณ , ๋ ์ด์์๋ ๋งค๋ฒ ์ด๊ธฐํํ๋ ๊ฒ์ด ์๋ ์ ์ฅ ํ๋กํผํฐ๋ก ๋ณ๊ฒฝํ๊ฒ๋ ์์ ํ์์ต๋๋ค.
    
```swift
private let listLayout: UICollectionViewFlowLayout = {
    let layout = UICollectionViewFlowLayout()
    layout.scrollDirection = .vertical
    layout.itemSize = CGSize(width: UIScreen.main.bounds.width - 20, height:
UIScreen.main.bounds.height / 12)
    layout.minimumLineSpacing = 0
    return layout
}()
private let gridLayout: UICollectionViewFlowLayout = {
    let layout = UICollectionViewFlowLayout()
    layout.scrollDirection = .vertical
    layout.itemSize = CGSize(width: UIScreen.main.bounds.width / 2 - 15,
                             height: UIScreen.main.bounds.height / 3)
    layout.sectionInset = .init(top: 10, left: 0, bottom: 0, right: 0)
    return layout
}()
private let collectionView: UICollectionView = {
    let collectionView = UICollectionView(frame: .zero, collectionViewLayout:
UICollectionViewLayout())
    collectionView.register(ListCell.self, forCellWithReuseIdentifier: "ListCell")
    collectionView.register(GridCell.self, forCellWithReuseIdentifier: "GridCell")
    collectionView.contentInset = UIEdgeInsets(top: .zero, left: 10, bottom: .zero, right:
10)
    collectionView.translatesAutoresizingMaskIntoConstraints = false
    return collectionView
}()
```

</details>
        
#### ๐ญ ๋ ์ด์์ ๋ณ๊ฒฝ์ ์คํฌ๋กค ๋๊ธฐํํ๊ธฐ

<details>
<summary> 
ํผ์ณ๋ณด๊ธฐ
</summary>

**๊ณ ๋ฏผ ๐ค**
- List์ Grid์ ๋ ํ๋ฉด์ ์ค๊ฐ๋ ์๋ก ๋ค๋ฅธ ์์ดํ์ ๋ณด๊ฒ๋๋ ๊ฒ๋ณด๋ค ๊ฐ์ ์์ดํ์ ๋ ์ด์์๋ง ๋ฌ๋ฆฌ ๋ณด๊ฒํ๋ ๊ฒ์ด ๋์ฑ ์ข์ ์ฌ์ฉ์ ๊ฒฝํ์ ์ ๋ฐํ๋ฆฌ๋ผ ์๊ฐํ์ต๋๋ค.
- ์ ์ ํ ์์น๋ก ์คํฌ๋กค์ ๋ง์ถ๊ธฐ ์ํด ์ฒ์์๋ `visibleCells` ํ๋กํผํฐ๋ฅผ ํ์ฉํ๊ณ ์ ํ์์ผ๋ ์ด๋ ์ ๋ ฌ๋์ง ์์ UICollectionViewCell์ ๋ฐฐ์ด์ ๋ฐํํ์์ต๋๋ค.
- ๋งค๋ฒ ๋์ผํ ๊ฒฐ๊ณผ๋ฅผ ๋ด๊ธฐ ์ํ์ฌ `indexPathsForVisibleItems.sprted()`๋ฅผ ์ฌ์ฉํด ์ค์ ๋ก ๋ณด์ด๋ ์ฒซ ๋ฒ์งธ ์์ดํ์ ์๋จ์ผ๋ก ์คํฌ๋กค์ ๋๊ธฐํ์์ผฐ์ต๋๋ค.
    
```swift
@objc private func changeLayout(_ segmentedControl: UISegmentedControl) {
    let visiblePath: [IndexPath] = collectionView.indexPathsForVisibleItems.sorted()
    var index: IndexPath = IndexPath()
    
    switch segmentedControl.selectedSegmentIndex {
    case LayoutType.list.rawValue:
        index = visiblePath.count == 8 ? visiblePath[2] : visiblePath[0]
        collectionView.collectionViewLayout = listLayout
    case LayoutType.grid.rawValue:
        index = collectionView.contentOffset.y > 0 ? visiblePath[2] : visiblePath[0]
        collectionView.collectionViewLayout = gridLayout
    default:
        break
    }
    collectionView.reloadData()
    collectionView.scrollToItem(at: index, at: .top, animated: false)
}
```
    
</details>
    
#### ๐ ์ํ ์์  ์๋ฃ์ ์์ ๋ ์ ๋ณด๊ฐ ๋ณด์ด์ง ์๋ ๋ฌธ์ 
    
<details>
<summary> 
ํผ์ณ๋ณด๊ธฐ
</summary>

**๋ฌธ์  ๐ป**
- ์ํ ์์ธํ๋ฉด์์ ์์  ๋ฒํผ์ ๋๋ฌ ์์ ์ ์งํํ ํ ์์ ์ด ์ฑ๊ณต์ ์ผ๋ก ์ด๋ฃจ์ด์ง๋ฉด ์ํ ์์ ํ๋ฉด์ด dismiss๋ฉ๋๋ค.
- ์ด ๋, ์ํ ์์ ํ๋ฉด์ด dismiss๋ ํ ๋ค์ ๋ํ๋ ์ํ ์์ธํ๋ฉด์์ ์ํ ์ ๋ณด๋ฅผ ์์ ํ๊ธฐ ์ด์  ๋ด์ฉ์ ๋ณด์ฌ์ฃผ๋ ๋ฌธ์ ๊ฐ ์์์ต๋๋ค.
    
**ํด๊ฒฐ ๐ซ**
- ๊ธฐ์กด์๋ ์ด๋ฐ ์ฌ์ฉ์ ๊ฒฝํ์ ๊ณ ๋ คํ์ง ์๊ณ  ์์์ ์งํํ๊ธฐ์ `viewDidLoad`์์ ์ํ ์ ๋ณด๋ฅผ ๋ฐ๋ ๋ก์ง์ ๊ตฌํํ์์ต๋๋ค.
- ์ด๋ฌํ UX๋ฅผ ๊ฐ์ ํ๊ธฐ ์ํด `viewDidLoad`๊ฐ ์๋ `viewWillAppear`์์ ์ํ ์์  ๋คํธ์ํน์ด ์๋ฃ๋ Response์ ๋ฐ์ดํฐ๋ฅผ ๋ณด์ฌ์ฃผ๋๋ก ๋ค์ ๊ตฌํํด ๋ณด์์ต๋๋ค.
    
```swift
override func viewWillAppear(_ animated: Bool) {
    super.viewWillAppear(animated)
        
    guard let request = ProductDetailRequest(productID: productID).request
    else { return }
    
    networkManager.fetchData(from: request, dataType: DetailProduct.self) { result in
        switch result {
        case .success(let data):
            self.detailProduct = data
            DispatchQueue.main.async {
                self.navigationItem.title = self.detailProduct?.name
                self.configureDetailView(detailProduct: data)
                self.setupImages(data.images)
            }
        case .failure(let error):
            print(error.localizedDescription)
        }
    }
}
```
</details>
    
#### ๐ญ ๋คํธ์ํน์ ํตํด ๋ฐ์์จ DTO ํ์ผ์ ๋ณํฉ

<details>
<summary> 
ํผ์ณ๋ณด๊ธฐ
</summary>

**๊ณ ๋ฏผ ๐ค**
- ๊ธฐ์กด `NewProduct`์ `EditProduct`์ ๊ฒฝ์ฐ, ๋น์ทํ ๊ฐ์ด ๋ง๊ณ  ์ฌ์ฉํ๋ ๋ฐฉ์๋ํ ๋น์ทํด ์ด ๋์ ํฉ์น๋ ๊ฒ์ด ๋ ์ข์ ๋ฐฉํฅ์ด ์๋๊น ํ๋ ๊ณ ๋ฏผ์ ํ์์ต๋๋ค.
- ๋๋ฌธ์ ์ฌ๋ฌ DTO๋ฅผ ์ ๊ฒํ๊ณ  ํ๋๋ก ํตํฉํ  ์ ์๋ DTO๋ผ๋ฆฌ ํตํฉํ์ฌ ์ฝ๋์ ๊ฐ๋์ฑ์ ๋์ด๊ณ , ๋ถํ์ํ ์ค๋ณต์ ์ค์ด๋ ๋ฐฉํฅ์ผ๋ก ๋ฆฌํฉํ ๋งํ์์ต๋๋ค. 
- ๊ฒฐ๊ณผ์ ์ผ๋ก `NewProduct`์ `EditProduct`์ ํ๋์ `SendingProduct`๋ผ๋ ๊ฐ์ฒด๋ก ํตํฉํ์ฌ ๊ด๋ฆฌํ๊ฒ ๋์์ต๋๋ค.
    
```swift
struct SendingProduct: Encodable {
    let productID: Int?
    let name, description: String
    let stock: Int
    let thumbnailID: Int?
    let discountedPrice, price: Double
    let currency: Currency
    let secret: String
    
    // CodingKeys ๋ฐ ์ด๋์๋ผ์ด์ ..
}
```
    
</details>
    
## ๐ ์ฐธ๊ณ  ๋งํฌ

[๊ณต์๋ฌธ์]

- [Apple Developer Documentation - URLSession](https://developer.apple.com/documentation/foundation/urlsession)
- [Apple Developer Documentation - Fetching Website Data into Memory](https://developer.apple.com/documentation/foundation/url_loading_system/fetching_website_data_into_memory)
- [Apple Developer Documentation - UICollectionView](https://developer.apple.com/documentation/uikit/uicollectionview)
- [Apple Developer Documentation - UIAlertController](https://developer.apple.com/documentation/uikit/uialertcontroller)
- [Apple Developer HIG - Entering data](https://developer.apple.com/design/human-interface-guidelines/patterns/entering-data/)
- [WWDC2020 - Modern cell configuration](https://developer.apple.com/videos/play/wwdc2020/10027/)
- [WWDC2020 - Lists in UICollectionView](https://developer.apple.com/videos/play/wwdc2020/10026)
- [Implementing Modern Collection Views](https://developer.apple.com/documentation/uikit/views_and_controls/collection_views/implementing_modern_collection_views)

---

[โฌ๏ธ ๋งจ ์๋ก ์ด๋ํ๊ธฐ](#-open-market)
