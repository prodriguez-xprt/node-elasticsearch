# node-elasticsearch

## Getting Started

### Installation

1. First we need to install ElasticSearch, I did it via brew install but you can choose how to install it here [https://www.elastic.co](https://www.elastic.co/guide/en/elasticsearch/reference/current/install-elasticsearch.html)
    ```sh
    brew tap elastic/tap
    brew install elastic/tap/elasticsearch-full
    ```

2. Start elasticsearch service
   ```sh
   elasticsearch
   ```

3. Install node modules
   ```sh
   npm install
   ```

3. Start the project
   ```sh
   npm start
   ```

### Load Indexes into elasticsearch

1. Enter into Postman and do multiple **POST** request to the url `localhost:3000/api/v1/products` containing as body each of `the_products` elements inside `routes.js`

2. After that we can do get by any field inside each key of the `the_products` elements. Doing a GET API call for example doing this call with Postman using the url:
    ```sh
   localhost:3000/api/v1/products?product=hermoso
   ```
