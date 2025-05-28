# swagger_client.DefaultApi

All URIs are relative to *https://api.myecommerce.com/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**orders_get**](DefaultApi.md#orders_get) | **GET** /orders | Отримати список замовлень
[**orders_order_id_delete**](DefaultApi.md#orders_order_id_delete) | **DELETE** /orders/{orderId} | Видалити замовлення
[**orders_order_id_get**](DefaultApi.md#orders_order_id_get) | **GET** /orders/{orderId} | Отримати замовлення за ID
[**orders_order_id_put**](DefaultApi.md#orders_order_id_put) | **PUT** /orders/{orderId} | Оновити замовлення
[**orders_post**](DefaultApi.md#orders_post) | **POST** /orders | Створити нове замовлення
[**payments_get**](DefaultApi.md#payments_get) | **GET** /payments | Отримати список оплат
[**payments_payment_id_delete**](DefaultApi.md#payments_payment_id_delete) | **DELETE** /payments/{paymentId} | Скасувати оплату
[**payments_payment_id_get**](DefaultApi.md#payments_payment_id_get) | **GET** /payments/{paymentId} | Отримати оплату за ID
[**payments_payment_id_put**](DefaultApi.md#payments_payment_id_put) | **PUT** /payments/{paymentId} | Оновити оплату
[**payments_post**](DefaultApi.md#payments_post) | **POST** /payments | Зареєструвати оплату

# **orders_get**
> list[Order] orders_get()

Отримати список замовлень

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.DefaultApi()

try:
    # Отримати список замовлень
    api_response = api_instance.orders_get()
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->orders_get: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[Order]**](Order.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orders_order_id_delete**
> orders_order_id_delete(order_id)

Видалити замовлення

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.DefaultApi()
order_id = 'order_id_example' # str | 

try:
    # Видалити замовлення
    api_instance.orders_order_id_delete(order_id)
except ApiException as e:
    print("Exception when calling DefaultApi->orders_order_id_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_id** | **str**|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orders_order_id_get**
> orders_order_id_get(order_id)

Отримати замовлення за ID

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.DefaultApi()
order_id = 'order_id_example' # str | 

try:
    # Отримати замовлення за ID
    api_instance.orders_order_id_get(order_id)
except ApiException as e:
    print("Exception when calling DefaultApi->orders_order_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_id** | **str**|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orders_order_id_put**
> orders_order_id_put(body, order_id)

Оновити замовлення

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.DefaultApi()
body = swagger_client.Order() # Order | 
order_id = 'order_id_example' # str | 

try:
    # Оновити замовлення
    api_instance.orders_order_id_put(body, order_id)
except ApiException as e:
    print("Exception when calling DefaultApi->orders_order_id_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Order**](Order.md)|  | 
 **order_id** | **str**|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orders_post**
> orders_post(body)

Створити нове замовлення

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.DefaultApi()
body = swagger_client.Order() # Order | 

try:
    # Створити нове замовлення
    api_instance.orders_post(body)
except ApiException as e:
    print("Exception when calling DefaultApi->orders_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Order**](Order.md)|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **payments_get**
> list[Payment] payments_get()

Отримати список оплат

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.DefaultApi()

try:
    # Отримати список оплат
    api_response = api_instance.payments_get()
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->payments_get: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[Payment]**](Payment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **payments_payment_id_delete**
> payments_payment_id_delete(payment_id)

Скасувати оплату

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.DefaultApi()
payment_id = 'payment_id_example' # str | 

try:
    # Скасувати оплату
    api_instance.payments_payment_id_delete(payment_id)
except ApiException as e:
    print("Exception when calling DefaultApi->payments_payment_id_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **payment_id** | **str**|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **payments_payment_id_get**
> payments_payment_id_get(payment_id)

Отримати оплату за ID

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.DefaultApi()
payment_id = 'payment_id_example' # str | 

try:
    # Отримати оплату за ID
    api_instance.payments_payment_id_get(payment_id)
except ApiException as e:
    print("Exception when calling DefaultApi->payments_payment_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **payment_id** | **str**|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **payments_payment_id_put**
> payments_payment_id_put(body, payment_id)

Оновити оплату

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.DefaultApi()
body = swagger_client.Payment() # Payment | 
payment_id = 'payment_id_example' # str | 

try:
    # Оновити оплату
    api_instance.payments_payment_id_put(body, payment_id)
except ApiException as e:
    print("Exception when calling DefaultApi->payments_payment_id_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Payment**](Payment.md)|  | 
 **payment_id** | **str**|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **payments_post**
> payments_post(body)

Зареєструвати оплату

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.DefaultApi()
body = swagger_client.Payment() # Payment | 

try:
    # Зареєструвати оплату
    api_instance.payments_post(body)
except ApiException as e:
    print("Exception when calling DefaultApi->payments_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Payment**](Payment.md)|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

