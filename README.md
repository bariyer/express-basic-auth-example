<h1 align="center">
  <code>@bariyer/express</code></br>
  basic authentication example
</h1>
<p align="center">
  <img width="256" alt="bariyer sub brand express logo" src="https://user-images.githubusercontent.com/29407019/134476716-61a6cff3-8122-4c45-bb10-669406702d6e.png">
</p>

<p align="center">
  <a href="https://github.com/bariyer/express-basic-auth-example/issues/new?assignees=&labels=Bug&title=">
    Report Bug
  </a>
  &nbsp;•&nbsp;
  <a href="https://github.com/bariyer/express-basic-auth-example/issues/new?assignees=&labels=Feature&title=">
    Request Feature
  </a>
</p>

## Installation
#### 1. Clone the repository
  ```bash
  git clone https://github.com/bariyer/express-basic-auth-example.git
  ```

#### 2. Install dependencies
  ```bash
  npm i
  ```
  ```bash
  yarn
  ```

#### 3. Rename `.env.example` to `.env` and fill the values
  ```bash
  mv .env.example .env
  ```

  Example: 
  ```dotenv
  PORT=3000
  BASIC_AUTH_USERNAME=admin
  BASIC_AUTH_PASSWORD=admin
  ```

#### 3. Run the example server
  ```bash
  yarn start
  ```
  ```bash
  npm start
  ```

#### 4. Open [Postman](https://www.postman.com/) or similar tool to test the API

#### For Postman users
1. Import [postman collection](bariyer-express-basic-auth.postman_collection.json) in project root.
2. Run the basic auth request

#### For non-Postman users
`GET` [http://localhost:3000/](http://localhost:3000/)

##### Headers:
`Authorization: Basic am9objoxMjM0NTY=`
This is the base64 encoded string of `john:123456`
john is username and 123456 is password

#### 5. See the response
Response Code: `200 OK`
Response Body:
  ```json
  [
      {
          "id": 1,
          "name": "Milk"
      },
      {
          "id": 2,
          "name": "Cheese"
      }
  ]
  ```
## Contributing

- ##### If get an error, feel free to [open issue](https://github.com/bariyer/express-basic-auth-example/issues/new/choose).
- ##### If you have any questions, feel free to [open discussion](https://github.com/bariyer/express-basic-auth-example/discussions/new).

Contributions are what make the open source community such an amazing place to be inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feat/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feat/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See [`LICENSE`](LICENSE) for more information.