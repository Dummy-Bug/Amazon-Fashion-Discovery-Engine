# Amazon-Fashion-Discovery-Engine
Build a recommendation engine which suggests similar products (apparel) to the given product (apparel) in any e-commerce websites.
## Statement

Personalized product recommendations are the alternative way of navigating through the online shop. More people find products they need. Even if they didn’t think of them.

Build a recommendation engine which suggests  similar products to the given product  in any e-commerce websites ex. Amazon.com, myntra.com etc.

## Objective 

The recommendation engine, uses information about 1,80,000 products and  each product will have multiple features named

1. Title of the product  
2. Brand of the product
3. Color of the product
4. Type of the product
5. Image of the apparel , etc...

Data Source : amazon.com


[Implementation](https://github.com/Dummy-Bug/Amazon-Fashion-Discovery-Engine/blob/master/Amazon%20Fashion%20Discovery%20Engine.ipynb)

<h2> Features Used </h2>
  <ol>
  <li> asin  ( Amazon standard identification number) </li>
  <li> brand ( brand to which the product belongs to ) </li>
  <li> color ( Color information of apparel, it can contain many colors as   a value ex: red and black stripes ) </li>
  <li> product_type_name (type of the apperal, ex: SHIRT/TSHIRT ) </li>
  <li> medium_image_url  ( url of the image ) </li>
  <li> title (title of the product.) </li>
  <li> formatted_price (price of the product) </li>
  </ol>
  
 <h2>Flow</h2>

<ol>
    <li>Pre-Processing:</li>
        <ol>
            <li>Basic statistical Analysis</li>
            <li>De-duplication</li>
            <li>Text pre-processing</li>
        </ol>
    Observations: Title was filled with useful information and thus, quite important for recommendations.
    
<li>Recommendation Techniques:</li>
        <ol>
            <li>Text Based:</li>
            <ol>
                <li>Bag of Words</li>
                <li>Tf-idf</li>
                <li>idf</li>
            </ol>
            <li>Semantic Based:</li>
            <ol>
                <li>Avg Word2Vec</li>
                <li>Idf Weighted Word2Vec</li>
            </ol>
        </ol>
    <li>Features used for Recommendation:</li>
    <ol>
        <li>Title</li>
        <li>Brand</li>
        <li>Color</li>
        <li>Image</li>
        <li>Title+Brand+Color+Image Weighted</li>
        Observations: Idf-weighted Word2Vec technique for Title featurization resulted in best outcomes. And, Weighed schemes having different weights for title, color, brand and image helps to narrow down reasults based on certain combinations.
    </ol>
</ol>
