# Comparing `tmp/variational-0.4.1.tar.gz` & `tmp/variational-0.4.2.tar.gz`

## Comparing `variational-0.4.1.tar` & `variational-0.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 variational-0.4.1/requirements-test.txt
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 variational-0.4.1/requirements.txt
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 variational-0.4.1/tests/test_backoff.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 variational-0.4.1/tests/test_smoke.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 variational-0.4.1/variational/__init__.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 variational-0.4.1/variational/auth.py
--rw-r--r--   0        0        0    15334 2020-02-02 00:00:00.000000 variational-0.4.1/variational/client.py
--rw-r--r--   0        0        0    13246 2020-02-02 00:00:00.000000 variational-0.4.1/variational/models.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 variational-0.4.1/variational/paginate.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 variational-0.4.1/variational/permit.py
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 variational-0.4.1/variational/polling.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 variational-0.4.1/variational/wrappers.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 variational-0.4.1/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 variational-0.4.1/LICENSE
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 variational-0.4.1/README.md
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 variational-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 variational-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 variational-0.4.2/requirements-test.txt
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 variational-0.4.2/requirements.txt
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 variational-0.4.2/tests/test_backoff.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 variational-0.4.2/tests/test_smoke.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 variational-0.4.2/variational/__init__.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 variational-0.4.2/variational/auth.py
+-rw-r--r--   0        0        0    15339 2020-02-02 00:00:00.000000 variational-0.4.2/variational/client.py
+-rw-r--r--   0        0        0    13277 2020-02-02 00:00:00.000000 variational-0.4.2/variational/models.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 variational-0.4.2/variational/paginate.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 variational-0.4.2/variational/permit.py
+-rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 variational-0.4.2/variational/polling.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 variational-0.4.2/variational/wrappers.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 variational-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 variational-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 variational-0.4.2/README.md
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 variational-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 variational-0.4.2/PKG-INFO
```

### Comparing `variational-0.4.1/variational/auth.py` & `variational-0.4.2/variational/auth.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import hashlib
 import hmac
 import time
 
 import requests
 
 
-def sign_prepared_request(req: requests.PreparedRequest,
-                          key: str, secret: str) -> requests.PreparedRequest:
+def sign_prepared_request(
+    req: requests.PreparedRequest, key: str, secret: str
+) -> requests.PreparedRequest:
     timestamp_ms = int(time.time() * 1000)
     message = f"{key}|{timestamp_ms}|{req.method}|{req.path_url}"
     signer = hmac.new(bytes.fromhex(secret), message.encode(), hashlib.sha256)
 
     # if request has body, append another pipe and the entire request body as bytes
     if isinstance(req.body, bytes):
         # arguments need to implement Buffer protocol, so everything is bytes, not str
         signer.update(b"|")
         signer.update(req.body)
 
-    req.prepare_headers(dict(req.headers, **{
-        "X-Request-Timestamp-Ms": str(timestamp_ms),
-        "X-Variational-Key": key,
-        "X-Variational-Signature": signer.hexdigest(),
-    }))
+    req.prepare_headers(
+        dict(
+            req.headers,
+            **{
+                "X-Request-Timestamp-Ms": str(timestamp_ms),
+                "X-Variational-Key": key,
+                "X-Variational-Signature": signer.hexdigest(),
+            },
+        )
+    )
 
     return req
```

### Comparing `variational-0.4.1/variational/client.py` & `variational-0.4.2/variational/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,322 +3,485 @@
 import time
 from typing import Optional, Dict, Mapping, List
 from urllib.parse import urlencode
 
 import requests
 
 from .auth import sign_prepared_request
-from .models import (StrDecimal, DateTimeRFC3339, H160, Allowance, AssetToken, UUIDv4, Company,
-                     Address, SettlementPool, Asset, Position, AggregatedPosition, Trade, Transfer,
-                     PortfolioSummary, Quote, RFQ, SupportedAssetDetails, AuthContext, Status,
-                     Structure, PoolStrategy, LegQuote, QuoteAcceptResponse, MakerLastLookResponse,
-                     MarginParams, TradeSide, TransferType, RequestAction, StructurePriceResponse,
-                     Instrument, InstrumentPrice)
+from .models import (
+    StrDecimal,
+    DateTimeRFC3339,
+    H160,
+    Allowance,
+    AssetToken,
+    UUIDv4,
+    Company,
+    Address,
+    SettlementPool,
+    Asset,
+    Position,
+    AggregatedPosition,
+    Trade,
+    Transfer,
+    PortfolioSummary,
+    Quote,
+    RFQ,
+    SupportedAssetDetails,
+    AuthContext,
+    Status,
+    Structure,
+    PoolStrategy,
+    LegQuote,
+    QuoteAcceptResponse,
+    MakerLastLookResponse,
+    MarginParams,
+    TradeSide,
+    TransferType,
+    RequestAction,
+    StructurePriceResponse,
+    Instrument,
+    InstrumentPrice,
+)
 from .wrappers import ApiSingle, ApiList, ApiPage, ApiError
 
 RATE_LIMIT_RESET_MS_HEADER = "x-rate-limit-resets-in-ms"
 MAINNET = "https://api.variational.io/v1"
 TESTNET = "https://api.testnet.variational.io/v1"
 
 
 class Client(object):
-    def __init__(self, key: str, secret: str, base_url: str = MAINNET,
-                 request_timeout: Optional[float] = None, retry_rate_limits=True):
+    def __init__(
+        self,
+        key: str,
+        secret: str,
+        base_url: str = MAINNET,
+        request_timeout: Optional[float] = None,
+        retry_rate_limits=True,
+    ):
         self.sesh = requests.session()
         self.key = key
         self.secret = secret
         self.base_url = base_url
         self.logger = logging.getLogger(__name__)
         self.request_timeout = request_timeout
         self.retry_rate_limits = retry_rate_limits
 
-    def accept_quote(self, rfq_id: UUIDv4, parent_quote_id: UUIDv4,
-                     side: TradeSide) -> ApiSingle[QuoteAcceptResponse]:
+    def accept_quote(
+        self, rfq_id: UUIDv4, parent_quote_id: UUIDv4, side: TradeSide
+    ) -> ApiSingle[QuoteAcceptResponse]:
         payload = {
             "parent_quote_id": parent_quote_id,
             "rfq_id": rfq_id,
             "side": side,
         }
 
-        return ApiSingle.from_response(self.__send_request(endpoint="/quotes/accept",
-                                                           method="POST", payload=payload))
+        return ApiSingle.from_response(
+            self.__send_request(
+                endpoint="/quotes/accept", method="POST", payload=payload
+            )
+        )
 
     def cancel_all_quotes(self) -> ApiSingle[bool]:
-        return ApiSingle.from_response(self.__send_request(endpoint="/quotes/cancel_all",
-                                                           method="POST"))
+        return ApiSingle.from_response(
+            self.__send_request(endpoint="/quotes/cancel_all", method="POST")
+        )
 
     def cancel_quote(self, id: UUIDv4) -> ApiSingle[bool]:
-        payload = {'id': id}
-        return ApiSingle.from_response(self.__send_request(endpoint="/quotes/cancel",
-                                                           method="POST", payload=payload))
+        payload = {"id": id}
+        return ApiSingle.from_response(
+            self.__send_request(
+                endpoint="/quotes/cancel", method="POST", payload=payload
+            )
+        )
 
     def cancel_rfq(self, id: UUIDv4) -> ApiSingle[bool]:
-        payload = {'id': id}
-        return ApiSingle.from_response(self.__send_request(endpoint="/rfqs/cancel",
-                                                           method="POST", payload=payload))
-
-    def create_quote(self, rfq_id: UUIDv4, expires_at: DateTimeRFC3339, leg_quotes: List[LegQuote],
-                     pool_strategy: PoolStrategy,
-                     client_quote_id: Optional[str] = None) -> ApiSingle[Quote]:
+        payload = {"id": id}
+        return ApiSingle.from_response(
+            self.__send_request(endpoint="/rfqs/cancel", method="POST", payload=payload)
+        )
+
+    def create_quote(
+        self,
+        rfq_id: UUIDv4,
+        expires_at: DateTimeRFC3339,
+        leg_quotes: List[LegQuote],
+        pool_strategy: PoolStrategy,
+        client_quote_id: Optional[str] = None,
+    ) -> ApiSingle[Quote]:
         payload = {
             "rfq_id": rfq_id,
             "expires_at": expires_at,
             "leg_quotes": leg_quotes,
             "pool_strategy": pool_strategy,
             "client_quote_id": client_quote_id,
         }
 
-        return ApiSingle.from_response(self.__send_request(endpoint="/quotes/new",
-                                                           method="POST", payload=payload))
-
-    def create_rfq(self, structure: Structure, qty: StrDecimal, expires_at: DateTimeRFC3339,
-                   target_companies: List[UUIDv4]) -> ApiSingle[RFQ]:
-
+        return ApiSingle.from_response(
+            self.__send_request(endpoint="/quotes/new", method="POST", payload=payload)
+        )
+
+    def create_rfq(
+        self,
+        structure: Structure,
+        qty: StrDecimal,
+        expires_at: DateTimeRFC3339,
+        target_companies: List[UUIDv4],
+    ) -> ApiSingle[RFQ]:
         payload = {
             "structure": structure,
             "qty": qty,
             "expires_at": expires_at,
             "target_companies": target_companies,
         }
 
-        return ApiSingle.from_response(self.__send_request(endpoint="/rfqs/new",
-                                                           method="POST", payload=payload))
-
-    def create_settlement_pool(self, pool_name: str, company_other: UUIDv4,
-                               creator_params: MarginParams,
-                               other_params: MarginParams) -> ApiSingle[SettlementPool]:
+        return ApiSingle.from_response(
+            self.__send_request(endpoint="/rfqs/new", method="POST", payload=payload)
+        )
+
+    def create_settlement_pool(
+        self,
+        pool_name: str,
+        company_other: UUIDv4,
+        creator_params: MarginParams,
+        other_params: MarginParams,
+    ) -> ApiSingle[SettlementPool]:
         payload = {
             "pool_name": pool_name,
             "company_other": company_other,
             "creator_params": creator_params,
             "other_params": other_params,
         }
-        return ApiSingle.from_response(self.__send_request(endpoint="/settlement_pools/new",
-                                                           method="POST", payload=payload))
-
-    def create_transfer(self, asset: AssetToken, qty: StrDecimal,
-                        target_pool_location: UUIDv4,
-                        transfer_type: TransferType) -> ApiSingle[Transfer]:
+        return ApiSingle.from_response(
+            self.__send_request(
+                endpoint="/settlement_pools/new", method="POST", payload=payload
+            )
+        )
+
+    def create_transfer(
+        self,
+        asset: AssetToken,
+        qty: StrDecimal,
+        target_pool_location: UUIDv4,
+        transfer_type: TransferType,
+    ) -> ApiSingle[Transfer]:
         payload = {
-            'asset': asset,
-            'qty': qty,
-            'target_pool_location': target_pool_location,
-            'transfer_type': transfer_type,
+            "asset": asset,
+            "qty": qty,
+            "target_pool_location": target_pool_location,
+            "transfer_type": transfer_type,
         }
-        return ApiSingle.from_response(self.__send_request(endpoint="/transfers/new",
-                                                           method="POST", payload=payload))
-
-    def generate_transfer_permit(self, pool_address: H160, allowance: Allowance,
-                                 seconds_until_expiry: Optional[int] = None) -> ApiSingle[dict]:
+        return ApiSingle.from_response(
+            self.__send_request(
+                endpoint="/transfers/new", method="POST", payload=payload
+            )
+        )
+
+    def generate_transfer_permit(
+        self,
+        pool_address: H160,
+        allowance: Allowance,
+        seconds_until_expiry: Optional[int] = None,
+    ) -> ApiSingle[dict]:
         payload = {
             "pool_address": pool_address,
             "allowance": allowance,
             "seconds_until_expiry": seconds_until_expiry,
         }
-        return ApiSingle.from_response(self.__send_request(
-            endpoint="/transfers/permit/template", method="POST", payload=payload))
+        return ApiSingle.from_response(
+            self.__send_request(
+                endpoint="/transfers/permit/template", method="POST", payload=payload
+            )
+        )
 
     def get_addresses(self, company: Optional[UUIDv4] = None) -> ApiList[Address]:
         f = {}
         if company:
-            f['company'] = company
-        return ApiList.from_response(self.__send_request(endpoint="/addresses", filter=f))
-
-    def get_companies(self, id: Optional[UUIDv4] = None,
-                      page: Optional[Dict] = None) -> ApiPage[Company]:
+            f["company"] = company
+        return ApiList.from_response(
+            self.__send_request(endpoint="/addresses", filter=f)
+        )
+
+    def get_companies(
+        self, id: Optional[UUIDv4] = None, page: Optional[Dict] = None
+    ) -> ApiPage[Company]:
         filter = {}
         if id:
-            filter['id'] = id
-        return ApiPage.from_response(self.__send_request(endpoint="/companies",
-                                                         filter=filter, page=page))
+            filter["id"] = id
+        return ApiPage.from_response(
+            self.__send_request(endpoint="/companies", filter=filter, page=page)
+        )
 
     def get_me(self) -> ApiSingle[AuthContext]:
         return ApiSingle.from_response(self.__send_request(endpoint="/me"))
 
-    def get_portfolio_aggregated_positions(self,
-                                           page: Optional[Dict] = None
-                                           ) -> ApiPage[AggregatedPosition]:
-        return ApiPage.from_response(self.__send_request(
-            endpoint="/portfolio/positions/aggregated", page=page))
-
-    def get_portfolio_assets(self, pool: Optional[UUIDv4] = None,
-                             page: Optional[Dict] = None) -> ApiPage[Asset]:
+    def get_portfolio_aggregated_positions(
+        self, page: Optional[Dict] = None
+    ) -> ApiPage[AggregatedPosition]:
+        return ApiPage.from_response(
+            self.__send_request(endpoint="/portfolio/positions/aggregated", page=page)
+        )
+
+    def get_portfolio_assets(
+        self, pool: Optional[UUIDv4] = None, page: Optional[Dict] = None
+    ) -> ApiPage[Asset]:
         filter = {}
         if pool:
-            filter['pool'] = pool
-        return ApiPage.from_response(self.__send_request(endpoint="/portfolio/assets",
-                                                         filter=filter, page=page))
-
-    def get_portfolio_positions(self, pool: Optional[UUIDv4] = None,
-                                page: Optional[Dict] = None) -> ApiPage[Position]:
+            filter["pool"] = pool
+        return ApiPage.from_response(
+            self.__send_request(endpoint="/portfolio/assets", filter=filter, page=page)
+        )
+
+    def get_portfolio_positions(
+        self, pool: Optional[UUIDv4] = None, page: Optional[Dict] = None
+    ) -> ApiPage[Position]:
         filter = {}
         if pool:
-            filter['pool'] = pool
-        return ApiPage.from_response(self.__send_request(endpoint="/portfolio/positions",
-                                                         filter=filter, page=page))
+            filter["pool"] = pool
+        return ApiPage.from_response(
+            self.__send_request(
+                endpoint="/portfolio/positions", filter=filter, page=page
+            )
+        )
 
     def get_portfolio_summary(self) -> ApiSingle[PortfolioSummary]:
-        return ApiSingle.from_response(self.__send_request(endpoint="/portfolio/summary"))
-
-    def get_portfolio_trades(self, pool: Optional[UUIDv4] = None, id: Optional[UUIDv4] = None,
-                             page: Optional[Dict] = None) -> ApiPage[Trade]:
+        return ApiSingle.from_response(
+            self.__send_request(endpoint="/portfolio/summary")
+        )
+
+    def get_portfolio_trades(
+        self,
+        pool: Optional[UUIDv4] = None,
+        id: Optional[UUIDv4] = None,
+        page: Optional[Dict] = None,
+    ) -> ApiPage[Trade]:
         filter = {}
         if pool:
-            filter['pool'] = pool
+            filter["pool"] = pool
         if id:
-            filter['id'] = id
-        return ApiPage.from_response(self.__send_request(endpoint="/portfolio/trades",
-                                                         filter=filter, page=page))
-
-    def get_transfers(self, pool: Optional[UUIDv4] = None, id: Optional[UUIDv4] = None,
-                      page: Optional[Dict] = None) -> ApiPage[Transfer]:
+            filter["id"] = id
+        return ApiPage.from_response(
+            self.__send_request(endpoint="/portfolio/trades", filter=filter, page=page)
+        )
+
+    def get_transfers(
+        self,
+        pool: Optional[UUIDv4] = None,
+        id: Optional[UUIDv4] = None,
+        page: Optional[Dict] = None,
+    ) -> ApiPage[Transfer]:
         filter = {}
         if pool:
-            filter['pool'] = pool
+            filter["pool"] = pool
         if id:
-            filter['id'] = id
-        return ApiPage.from_response(self.__send_request(endpoint="/transfers",
-                                                         filter=filter, page=page))
-
-    def get_quotes(self, id: Optional[UUIDv4] = None,
-                   page: Optional[Dict] = None) -> ApiPage[Quote]:
+            filter["id"] = id
+        return ApiPage.from_response(
+            self.__send_request(endpoint="/transfers", filter=filter, page=page)
+        )
+
+    def get_quotes(
+        self, id: Optional[UUIDv4] = None, page: Optional[Dict] = None
+    ) -> ApiPage[Quote]:
         filter = {}
         if id:
-            filter['id'] = id
-        return ApiPage.from_response(self.__send_request(endpoint="/quotes",
-                                                         filter=filter, page=page))
-
-    def get_quotes_received(self, id: Optional[UUIDv4] = None,
-                            page: Optional[Dict] = None) -> ApiPage[Quote]:
+            filter["id"] = id
+        return ApiPage.from_response(
+            self.__send_request(endpoint="/quotes", filter=filter, page=page)
+        )
+
+    def get_quotes_received(
+        self, id: Optional[UUIDv4] = None, page: Optional[Dict] = None
+    ) -> ApiPage[Quote]:
         filter = {}
         if id:
-            filter['id'] = id
-        return ApiPage.from_response(self.__send_request(endpoint="/quotes/received",
-                                                         filter=filter, page=page))
-
-    def get_quotes_sent(self, id: Optional[UUIDv4] = None,
-                        page: Optional[Dict] = None) -> ApiPage[Quote]:
+            filter["id"] = id
+        return ApiPage.from_response(
+            self.__send_request(endpoint="/quotes/received", filter=filter, page=page)
+        )
+
+    def get_quotes_sent(
+        self, id: Optional[UUIDv4] = None, page: Optional[Dict] = None
+    ) -> ApiPage[Quote]:
         filter = {}
         if id:
-            filter['id'] = id
-        return ApiPage.from_response(self.__send_request(endpoint="/quotes/sent",
-                                                         filter=filter, page=page))
-
-    def get_rfqs_received(self, id: Optional[UUIDv4] = None,
-                          page: Optional[Dict] = None) -> ApiPage[RFQ]:
+            filter["id"] = id
+        return ApiPage.from_response(
+            self.__send_request(endpoint="/quotes/sent", filter=filter, page=page)
+        )
+
+    def get_rfqs_received(
+        self,
+        id: Optional[UUIDv4] = None,
+        page: Optional[Dict] = None,
+        price: Optional[bool] = None,
+    ) -> ApiPage[RFQ]:
         filter = {}
         if id:
-            filter['id'] = id
-        return ApiPage.from_response(self.__send_request(endpoint="/rfqs/received",
-                                                         filter=filter, page=page))
-
-    def get_rfqs_sent(self, id: Optional[UUIDv4] = None,
-                      page: Optional[Dict] = None) -> ApiPage[RFQ]:
+            filter["id"] = id
+        if price is None or price:
+            filter["price"] = "true"
+        else:
+            filter["price"] = "false"
+        return ApiPage.from_response(
+            self.__send_request(endpoint="/rfqs/received", filter=filter, page=page)
+        )
+
+    def get_rfqs_sent(
+        self,
+        id: Optional[UUIDv4] = None,
+        page: Optional[Dict] = None,
+        price: Optional[bool] = None,
+    ) -> ApiPage[RFQ]:
         filter = {}
         if id:
-            filter['id'] = id
-        return ApiPage.from_response(self.__send_request(endpoint="/rfqs/sent",
-                                                         filter=filter, page=page))
-
-    def get_settlement_pools(self, id: Optional[UUIDv4] = None,
-                             page: Optional[Dict] = None) -> ApiPage[SettlementPool]:
+            filter["id"] = id
+        if price is None or price:
+            filter["price"] = "true"
+        else:
+            filter["price"] = "false"
+        return ApiPage.from_response(
+            self.__send_request(endpoint="/rfqs/sent", filter=filter, page=page)
+        )
+
+    def get_settlement_pools(
+        self, id: Optional[UUIDv4] = None, page: Optional[Dict] = None
+    ) -> ApiPage[SettlementPool]:
         filter = {}
         if id:
-            filter['id'] = id
-        return ApiPage.from_response(self.__send_request(endpoint="/settlement_pools",
-                                                         filter=filter, page=page))
+            filter["id"] = id
+        return ApiPage.from_response(
+            self.__send_request(endpoint="/settlement_pools", filter=filter, page=page)
+        )
 
     def get_status(self) -> ApiSingle[Status]:
         return ApiSingle.from_response(self.__send_request(endpoint="/status"))
 
-    def get_supported_assets(self, verified: Optional[bool] = False) \
-            -> ApiSingle[Dict[AssetToken, List[SupportedAssetDetails]]]:
+    def get_supported_assets(
+        self, verified: Optional[bool] = False
+    ) -> ApiSingle[Dict[AssetToken, List[SupportedAssetDetails]]]:
         filter = {}
         if verified:
-            filter['verified'] = 'true'
-        return ApiSingle.from_response(self.__send_request(
-            endpoint="/metadata/supported_assets", filter=filter))
-
-    def maker_last_look(self, rfq_id: UUIDv4, parent_quote_id: UUIDv4,
-                        action: RequestAction) -> ApiSingle[MakerLastLookResponse]:
+            filter["verified"] = "true"
+        return ApiSingle.from_response(
+            self.__send_request(endpoint="/metadata/supported_assets", filter=filter)
+        )
+
+    def maker_last_look(
+        self, rfq_id: UUIDv4, parent_quote_id: UUIDv4, action: RequestAction
+    ) -> ApiSingle[MakerLastLookResponse]:
         payload = {
             "parent_quote_id": parent_quote_id,
             "rfq_id": rfq_id,
             "action": action,
         }
-        return ApiSingle.from_response(self.__send_request(endpoint="/quotes/maker_last_look",
-                                                           method="POST", payload=payload))
+        return ApiSingle.from_response(
+            self.__send_request(
+                endpoint="/quotes/maker_last_look", method="POST", payload=payload
+            )
+        )
 
     def price_instrument(self, instrument: Instrument) -> ApiSingle[InstrumentPrice]:
-        return ApiSingle.from_response(self.__send_request(
-            endpoint="/price/instrument", method="POST", payload=instrument))
-
-    def price_structure(self, structure: Structure) -> ApiSingle[StructurePriceResponse]:
-        return ApiSingle.from_response(self.__send_request(endpoint="/price/structure",
-                                                           method="POST", payload=structure))
-
-    def replace_quote(self, parent_quote_id: UUIDv4, rfq_id: UUIDv4, expires_at: DateTimeRFC3339,
-                      leg_quotes: List[LegQuote],
-                      pool_strategy: PoolStrategy,
-                      client_quote_id: Optional[str] = None) -> ApiSingle[Quote]:
+        return ApiSingle.from_response(
+            self.__send_request(
+                endpoint="/price/instrument", method="POST", payload=instrument
+            )
+        )
+
+    def price_structure(
+        self, structure: Structure
+    ) -> ApiSingle[StructurePriceResponse]:
+        return ApiSingle.from_response(
+            self.__send_request(
+                endpoint="/price/structure", method="POST", payload=structure
+            )
+        )
+
+    def replace_quote(
+        self,
+        parent_quote_id: UUIDv4,
+        rfq_id: UUIDv4,
+        expires_at: DateTimeRFC3339,
+        leg_quotes: List[LegQuote],
+        pool_strategy: PoolStrategy,
+        client_quote_id: Optional[str] = None,
+    ) -> ApiSingle[Quote]:
         payload = {
             "parent_quote_id": parent_quote_id,
             "rfq_id": rfq_id,
             "expires_at": expires_at,
             "leg_quotes": leg_quotes,
             "pool_strategy": pool_strategy,
             "client_quote_id": client_quote_id,
         }
 
-        return ApiSingle.from_response(self.__send_request(endpoint="/quotes/replace",
-                                                           method="POST", payload=payload))
+        return ApiSingle.from_response(
+            self.__send_request(
+                endpoint="/quotes/replace", method="POST", payload=payload
+            )
+        )
 
     def submit_transfer_permit(self, message: dict, signature: str) -> ApiSingle[bool]:
         payload = {
             "message": message,
             "signature": signature,
         }
-        return ApiSingle.from_response(self.__send_request(endpoint="/transfers/permit",
-                                                           method="POST", payload=payload))
-
-    def __send_request(self, endpoint: str, method: str = "GET",
-                       payload: Optional[Dict | List] = None, filter: Optional[Dict] = None,
-                       page: Optional[Dict] = None) -> requests.Response:
+        return ApiSingle.from_response(
+            self.__send_request(
+                endpoint="/transfers/permit", method="POST", payload=payload
+            )
+        )
+
+    def __send_request(
+        self,
+        endpoint: str,
+        method: str = "GET",
+        payload: Optional[Dict | List] = None,
+        filter: Optional[Dict] = None,
+        page: Optional[Dict] = None,
+    ) -> requests.Response:
         params = {}
         if filter:
             params.update(filter)
         if page:
             params.update(page)
 
-        qs = ("?" + urlencode(params)) if params else ''
+        qs = ("?" + urlencode(params)) if params else ""
         backoff = ExpBackoff()
 
         full_url = self.base_url + endpoint + qs
         while True:
             req = requests.Request(method=method, url=full_url, json=payload).prepare()
-            resp = self.sesh.send(sign_prepared_request(req, self.key, self.secret),
-                                  timeout=self.request_timeout)
+            resp = self.sesh.send(
+                sign_prepared_request(req, self.key, self.secret),
+                timeout=self.request_timeout,
+            )
 
             if resp.status_code == 200:
                 return resp
 
             if self.retry_rate_limits and resp.status_code == 429:
                 if resets_in := _get_rate_limit_reset_timestamp(resp.headers):
                     # delay for at least the amount specified in the header
                     # add an extra delay that's slowly increasing with each attempt
                     delay = resets_in + backoff.next_delay()
 
-                    self.logger.warning("HTTP 429 Too Many Requests was returned from the API, "
-                                        "will retry after delay: %.3fs", delay)
+                    self.logger.warning(
+                        "HTTP 429 Too Many Requests was returned from the API, "
+                        "will retry after delay: %.3fs",
+                        delay,
+                    )
                     time.sleep(delay)
                     continue
 
             data = resp.json()
-            raise ApiError(url=full_url, status_code=resp.status_code,
-                           api_code=data['error']['code'], message=data['error']['message'])
+            raise ApiError(
+                url=full_url,
+                status_code=resp.status_code,
+                api_code=data["error"]["code"],
+                message=data["error"]["message"],
+            )
 
 
 class ExpBackoff:
     def __init__(self, base=0.2, factor=1.2, randomize=0.2):
         self.base = base
         self.factor = factor
         self.randomize = randomize
```

### Comparing `variational-0.4.1/variational/models.py` & `variational-0.4.2/variational/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 H160: TypeAlias = str  # e.g. "0x3d68316712565ccb7f14a2bfc6aa785d6d2d12d5"
 StrDecimal: TypeAlias = str  # e.g. "218205.58082"
 UUIDv4: TypeAlias = str  # e.g. "bdd68c99-65fe-4500-baae-5bc09b4af183"
 
 
 # Enums
 
+
 class ApiRole(StrEnum):
     READER = "reader"
     WRITER = "writer"
 
 
 class AllowanceType(StrEnum):
     BASE = "base"
@@ -118,27 +119,28 @@
     LIQUIDATION = "liquidation"
     REALIZED_PNL = "realized_pnl"
     INITIAL_MARGIN = "initial_margin"
 
 
 # Nested models
 
+
 class ClearingEvent(TypedDict):
     rfq_id: UUIDv4
     parent_quote_id: UUIDv4
     status: ClearingStatus
     created_at: DateTimeRFC3339
     taker_side: Optional[TradeSide]
 
 
 class CreateNewPool(TypedDict):
     strategy: PoolStrategyType  # = CREATE_NEW
     name: str  # length ∈ [1, 50]
-    creator_params: 'MarginParams'
-    other_params: 'MarginParams'
+    creator_params: "MarginParams"
+    other_params: "MarginParams"
 
 
 class DatedFuture(TypedDict):
     instrument_type: InstrumentType  # = DATED_FUTURE
     underlying: str  # ∈ {'BTC', 'ETH'}
     settlement_asset: str  # = 'USDC'
     expiry: DateTimeRFC3339  # date in the future or datetime at 08:00:00Z
@@ -159,34 +161,36 @@
     min_imbalance_dollars: StrDecimal
     funding_exponent_factor: StrDecimal
 
 
 class Leg(TypedDict):
     side: TradeSide
     ratio: int  # ≥ 1
-    instrument: 'Instrument'
+    instrument: "Instrument"
 
 
 class MarginUsage(TypedDict):
     initial_margin: StrDecimal
     maintenance_margin: StrDecimal
 
 
 class PerpetualFuture(TypedDict):
     instrument_type: InstrumentType  # = PERPETUAL_FUTURE
     underlying: str
     settlement_asset: str  # = 'USDC'
     funding_interval_s: int  # = 3600
-    dex_token_details: Optional[DexTokenDetails]  # required if underlying is a DEX token
+    dex_token_details: Optional[
+        DexTokenDetails
+    ]  # required if underlying is a DEX token
 
 
 class PoolMarginUsageStats(TypedDict):
     company: UUIDv4
     balance: StrDecimal
-    margin_params: 'MarginParams'
+    margin_params: "MarginParams"
     margin_usage: MarginUsage
 
 
 class PortfolioMarginAssetParam(TypedDict):
     vol_range_up: StrDecimal  # ∈ [0, 1]
     vol_range_down: StrDecimal  # ∈ [0, 1]
     short_vega_power: StrDecimal  # ∈ [0, 1]
@@ -215,20 +219,20 @@
 class QuoteCommonMetadata(TypedDict):
     parent_quote_id: UUIDv4
     maker_company: UUIDv4
     clearing_status: Optional[ClearingStatus]
     expires_at: DateTimeRFC3339
     pool_location: Optional[UUIDv4]
     new_pool_name: Optional[str]
-    creator_params: Optional['MarginParams']
-    other_params: Optional['MarginParams']
+    creator_params: Optional["MarginParams"]
+    other_params: Optional["MarginParams"]
     pool_creator_company: Optional[UUIDv4]
     pool_other_company: Optional[UUIDv4]
-    pool_creator_params: Optional['MarginParams']
-    pool_other_params: Optional['MarginParams']
+    pool_creator_params: Optional["MarginParams"]
+    pool_other_params: Optional["MarginParams"]
     clearing_events: List[ClearingEvent]
 
 
 class QuoteWithMarginRequirements(TypedDict):
     parent_quote_id: UUIDv4
     quote_price: StrDecimal
     counter_factual_margin_requirements: Optional[MarginUsage]
@@ -237,26 +241,26 @@
     margin_requirements_counter_factual_request_id: UUIDv4
     existing_margin_requirements_request_id: UUIDv4
 
 
 class RFQLeg(TypedDict):
     rfq_leg_id: UUIDv4
     rfq_id: UUIDv4
-    instrument: 'Instrument'
+    instrument: "Instrument"
     side: TradeSide
     qty: StrDecimal
 
 
 class SettlementPoolData(TypedDict):
     status: SettlementPoolStatus
     pool_name: str
     pool_address: Optional[H160]
     creator_address: H160
     other_address: H160
-    positions: List['AggregatedPosition']
+    positions: List["AggregatedPosition"]
     creator_company_margin_usage: PoolMarginUsageStats
     other_company_margin_usage: PoolMarginUsageStats
 
 
 class SimpleMarginAssetParam(TypedDict):
     futures_initial_margin: StrDecimal  # ∈ [0, 1]
     futures_maintenance_margin: StrDecimal  # ∈ [0, 1]
@@ -278,15 +282,17 @@
     params: SimpleMarginParams
 
 
 class Spot(TypedDict):
     instrument_type: InstrumentType  # = SPOT
     underlying: str
     settlement_asset: str  # = 'USDC'
-    dex_token_details: Optional[DexTokenDetails]  # required if underlying is a DEX token
+    dex_token_details: Optional[
+        DexTokenDetails
+    ]  # required if underlying is a DEX token
 
 
 class StructurePrice(TypedDict):
     price: StrDecimal
     native_price: StrDecimal
     delta: StrDecimal
     gamma: StrDecimal
@@ -309,14 +315,15 @@
     strike: StrDecimal  # > 0
     payoff: PayoffType
     exercise: ExerciseType
 
 
 # Top-level models
 
+
 class Address(TypedDict):
     created_at: Optional[DateTimeRFC3339]
     company: UUIDv4
     address: H160
     enabled: bool
 
 
@@ -327,15 +334,15 @@
     sum_delta: StrDecimal
     sum_gamma: StrDecimal
     upnl: StrDecimal
     notional: StrDecimal
     sum_rho: StrDecimal
     sum_theta: StrDecimal
     sum_vega: StrDecimal
-    position_info: 'Position'
+    position_info: "Position"
 
 
 class Allowance(TypedDict):
     type: AllowanceType
     value: StrDecimal | int
 
 
@@ -431,23 +438,23 @@
     other_params: Optional[MarginParams]
     pool_location: Optional[UUIDv4]
     per_leg_quotes: List[LegQuote]
 
 
 class QuoteAcceptResponse(TypedDict):
     pending_deposits_sum_qty: StrDecimal
-    pending_settlement_pool: Optional['SettlementPool']
+    pending_settlement_pool: Optional["SettlementPool"]
     new_clearing_status: ClearingStatus
 
 
 class RFQ(TypedDict):
     rfq_id: UUIDv4
     created_at: DateTimeRFC3339
     clearing_status: Optional[ClearingStatus]
-    structure: 'Structure'
+    structure: "Structure"
     structure_price: Optional[StructurePrice]
     rfq_expires_at: DateTimeRFC3339
     taker_company: UUIDv4
     rfq_status: RFQStatus
     qty: StrDecimal
     rfq_legs: List[RFQLeg]
     quotes_common_metadata: Dict[UUIDv4, QuoteCommonMetadata]
```

### Comparing `variational-0.4.1/variational/paginate.py` & `variational-0.4.2/variational/paginate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Callable, Generator
 
 from .wrappers import Pagination, ApiPage, T, ApiList
 
 
-def paginate(method: Callable[..., ApiPage[T]], *args, page=None,
-             **kwargs) -> Generator[T, None, None]:
+def paginate(
+    method: Callable[..., ApiPage[T]], *args, page=None, **kwargs
+) -> Generator[T, None, None]:
     next_pagination = Pagination(next_page=page)
     while True:
         wrapper = method(*args, page=next_pagination.next_page, **kwargs)
 
         if isinstance(wrapper, ApiPage):
             next_pagination = wrapper.pagination
         else:
```

### Comparing `variational-0.4.1/variational/permit.py` & `variational-0.4.2/variational/permit.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,49 +8,67 @@
 
 
 class TransferPermitHelper(object):
     def __init__(self, client: Client, private_key: str):
         self.client = client
         self.__private_key = private_key
 
-    def sign_and_submit_decimal(self, pool_address: H160, allowance: StrDecimal,
-                                seconds_until_expiry: Optional[int] = None):
+    def sign_and_submit_decimal(
+        self,
+        pool_address: H160,
+        allowance: StrDecimal,
+        seconds_until_expiry: Optional[int] = None,
+    ):
         return self._sign_and_submit(
             pool_address=pool_address,
             allowance={
-                'type': AllowanceType.DECIMAL,
-                'value': allowance,
+                "type": AllowanceType.DECIMAL,
+                "value": allowance,
             },
             seconds_until_expiry=seconds_until_expiry,
         )
 
-    def sign_and_submit_base(self, pool_address: H160, allowance: int,
-                             seconds_until_expiry: Optional[int] = None):
+    def sign_and_submit_base(
+        self,
+        pool_address: H160,
+        allowance: int,
+        seconds_until_expiry: Optional[int] = None,
+    ):
         return self._sign_and_submit(
             pool_address=pool_address,
             allowance={
-                'type': AllowanceType.BASE,
-                'value': allowance,
+                "type": AllowanceType.BASE,
+                "value": allowance,
             },
             seconds_until_expiry=seconds_until_expiry,
         )
 
-    def sign_and_submit_unlimited(self, pool_address: H160,
-                                  seconds_until_expiry: Optional[int] = None):
+    def sign_and_submit_unlimited(
+        self, pool_address: H160, seconds_until_expiry: Optional[int] = None
+    ):
         return self._sign_and_submit(
             pool_address=pool_address,
             allowance={
-                'type': AllowanceType.BASE,
-                'value': 2 ** 256 - 1,
+                "type": AllowanceType.BASE,
+                "value": 2**256 - 1,
             },
             seconds_until_expiry=seconds_until_expiry,
         )
 
-    def _sign_and_submit(self, pool_address: H160, allowance: Allowance,
-                         seconds_until_expiry: Optional[int] = None):
+    def _sign_and_submit(
+        self,
+        pool_address: H160,
+        allowance: Allowance,
+        seconds_until_expiry: Optional[int] = None,
+    ):
         msg = self.client.generate_transfer_permit(
             pool_address=pool_address,
             allowance=allowance,
-            seconds_until_expiry=seconds_until_expiry).result
-        msg['domain']['chainId'] = int(msg['domain']['chainId'], 16)
-        signed = Account.sign_message(encode_typed_data(full_message=msg), self.__private_key)
-        self.client.submit_transfer_permit(message=msg, signature=signed.signature.hex())
+            seconds_until_expiry=seconds_until_expiry,
+        ).result
+        msg["domain"]["chainId"] = int(msg["domain"]["chainId"], 16)
+        signed = Account.sign_message(
+            encode_typed_data(full_message=msg), self.__private_key
+        )
+        self.client.submit_transfer_permit(
+            message=msg, signature=signed.signature.hex()
+        )
```

### Comparing `variational-0.4.1/variational/polling.py` & `variational-0.4.2/variational/polling.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from time import sleep
 from typing import Callable, List
 
 from .client import Client
-from .models import (SettlementPoolStatus, TransferStatus, ClearingStatus, SettlementPool,
-                     Transfer, Quote, UUIDv4)
+from .models import (
+    SettlementPoolStatus,
+    TransferStatus,
+    ClearingStatus,
+    SettlementPool,
+    Transfer,
+    Quote,
+    UUIDv4,
+)
 
 
 class PollingHelper(object):
     def __init__(self, client: Client, interval=1, attempts=10):
         assert attempts > 0
         self.client = client
         self.interval = interval
@@ -17,87 +24,110 @@
             ClearingStatus.PENDING_TAKER_DEPOSIT_APPROVAL: 2,
             ClearingStatus.PENDING_MAKER_LAST_LOOK: 3,
             ClearingStatus.PENDING_MAKER_DEPOSIT_APPROVAL: 4,
             ClearingStatus.PENDING_ATOMIC_DEPOSIT: 5,
             ClearingStatus.SUCCESS_TRADES_BOOKED_INTO_POOL: 6,
         }
 
-    def wait_for_settlement_pool(self, pool_location: str,
-                                 status: SettlementPoolStatus = SettlementPoolStatus.OPEN) \
-            -> SettlementPool:
+    def wait_for_settlement_pool(
+        self,
+        pool_location: str,
+        status: SettlementPoolStatus = SettlementPoolStatus.OPEN,
+    ) -> SettlementPool:
         """
         Requests a settlement pool with the given `pool_location` until it reaches
         the desired status, returning the pool.
         Returns an error if a different final status is reached.
         Returns an error if runs out of attempts.
         """
         return self.__poll_for_status(
-            object_type='settlement pool',
+            object_type="settlement pool",
             object_id=pool_location,
             status=status,
-            fetch_objs=lambda: self.client.get_settlement_pools(id=pool_location).result,
-            get_status=lambda obj: obj['data']['status'],
+            fetch_objs=lambda: self.client.get_settlement_pools(
+                id=pool_location
+            ).result,
+            get_status=lambda obj: obj["data"]["status"],
             is_desired=lambda s: s == status,
-            is_final=lambda s: s in (SettlementPoolStatus.OPEN, SettlementPoolStatus.CANCELED)
+            is_final=lambda s: s
+            in (SettlementPoolStatus.OPEN, SettlementPoolStatus.CANCELED),
         )
 
-    def wait_for_transfer(self, id: str,
-                          status: TransferStatus = TransferStatus.CONFIRMED) -> Transfer:
+    def wait_for_transfer(
+        self, id: str, status: TransferStatus = TransferStatus.CONFIRMED
+    ) -> Transfer:
         """
         Requests a transfer with the given `id` until it reaches the desired status,
         returning the transfer.
         Returns an error if a different final status is reached.
         Returns an error if runs out of attempts.
         """
         return self.__poll_for_status(
-            object_type='transfer',
+            object_type="transfer",
             object_id=id,
             status=status,
             fetch_objs=lambda: self.client.get_transfers(id=id).result,
-            get_status=lambda obj: obj['status'],
+            get_status=lambda obj: obj["status"],
             is_desired=lambda s: s == status,
-            is_final=lambda s: s in (TransferStatus.CONFIRMED, TransferStatus.FAILED)
+            is_final=lambda s: s in (TransferStatus.CONFIRMED, TransferStatus.FAILED),
         )
 
-    def wait_for_clearing_status(self, parent_quote_id: UUIDv4, status: ClearingStatus) -> Quote:
+    def wait_for_clearing_status(
+        self, parent_quote_id: UUIDv4, status: ClearingStatus
+    ) -> Quote:
         """
         Requests a quote with the given `parent_quote_id` until it reaches the desired status
         or progresses beyond it, returning the quote.
         Returns an error if a different final status is reached.
         Returns an error if runs out of attempts.
         """
         return self.__poll_for_status(
-            object_type='quote',
+            object_type="quote",
             object_id=parent_quote_id,
             status=status,
             fetch_objs=lambda: self.client.get_quotes(id=parent_quote_id).result,
-            get_status=lambda obj: obj['clearing_status'],
+            get_status=lambda obj: obj["clearing_status"],
             is_desired=self._is_desired_clearing_status(status),
-            is_final=lambda s: (s == ClearingStatus.SUCCESS_TRADES_BOOKED_INTO_POOL or
-                                s is not None and s.startswith('rejected_'))
+            is_final=lambda s: (
+                s == ClearingStatus.SUCCESS_TRADES_BOOKED_INTO_POOL
+                or s is not None
+                and s.startswith("rejected_")
+            ),
         )
 
-    def _is_desired_clearing_status(self, desired: ClearingStatus) -> Callable[[str], bool]:
+    def _is_desired_clearing_status(
+        self, desired: ClearingStatus
+    ) -> Callable[[str], bool]:
         def _inner(current: ClearingStatus) -> bool:
             if current == desired:
                 return True
 
             ord_current = self.clearing_order.get(current)
             ord_desired = self.clearing_order.get(desired)
-            if (isinstance(ord_current, int) and isinstance(ord_desired, int)
-                    and ord_current >= ord_desired):
+            if (
+                isinstance(ord_current, int)
+                and isinstance(ord_desired, int)
+                and ord_current >= ord_desired
+            ):
                 return True
 
             return False
 
         return _inner
 
-    def __poll_for_status(self, object_type: str, object_id: str, status: str,
-                          fetch_objs: Callable[[], List[dict]], get_status: Callable[[dict], str],
-                          is_desired: Callable[[str], bool], is_final: Callable[[str], bool]):
+    def __poll_for_status(
+        self,
+        object_type: str,
+        object_id: str,
+        status: str,
+        fetch_objs: Callable[[], List[dict]],
+        get_status: Callable[[dict], str],
+        is_desired: Callable[[str], bool],
+        is_final: Callable[[str], bool],
+    ):
         for i in range(self.attempts):
             if i > 0:
                 sleep(self.interval)
 
             objs = fetch_objs()
             if len(objs) < 1:
                 raise ObjectNotFound(msg=f"{object_type} '{object_id}' not found")
@@ -107,19 +137,22 @@
 
             if is_desired(current_status):
                 return obj
 
             if is_final(current_status):
                 raise UnexpectedStatus(
                     msg=f"unexpected final status '{current_status}' "
-                        f"for {object_type} '{object_id}'",
-                    status=current_status)
-
-        raise PollTimeout(msg=f"timeout waiting for {object_type} '{object_id}'"
-                              f" to become '{status}'")
+                    f"for {object_type} '{object_id}'",
+                    status=current_status,
+                )
+
+        raise PollTimeout(
+            msg=f"timeout waiting for {object_type} '{object_id}'"
+            f" to become '{status}'"
+        )
 
 
 class ObjectNotFound(Exception):
     def __init__(self, msg: str):
         self.msg = msg
 
     def __str__(self):
```

### Comparing `variational-0.4.1/variational/wrappers.py` & `variational-0.4.2/variational/wrappers.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,31 +29,29 @@
 class ApiSingle(Generic[T]):
     result: T
     meta: ResponseMetadata
 
     @staticmethod
     def from_response(response: requests.Response):
         return ApiSingle(
-            result=response.json()['result'],
-            meta=ResponseMetadata(
-                _get_request_received_timestamp(response.headers)),
+            result=response.json()["result"],
+            meta=ResponseMetadata(_get_request_received_timestamp(response.headers)),
         )
 
 
 @dataclass
 class ApiList(Generic[T]):
     result: List[T]
     meta: ResponseMetadata
 
     @staticmethod
     def from_response(response: requests.Response):
         return ApiList(
-            result=response.json()['result'],
-            meta=ResponseMetadata(
-                _get_request_received_timestamp(response.headers)),
+            result=response.json()["result"],
+            meta=ResponseMetadata(_get_request_received_timestamp(response.headers)),
         )
 
 
 @dataclass
 class Pagination:
     next_page: Optional[Dict]
 
@@ -64,20 +62,18 @@
     pagination: Pagination
     meta: ResponseMetadata
 
     @staticmethod
     def from_response(response: requests.Response):
         data = response.json()
         return ApiPage(
-            result=data['result'],
-            pagination=Pagination(next_page=data['pagination']['next_page']),
-            meta=ResponseMetadata(
-                _get_request_received_timestamp(response.headers)),
+            result=data["result"],
+            pagination=Pagination(next_page=data["pagination"]["next_page"]),
+            meta=ResponseMetadata(_get_request_received_timestamp(response.headers)),
         )
 
 
 def _get_request_received_timestamp(headers: Mapping) -> Optional[float]:
     for k, v in headers.items():
         if k.lower() == RATE_LIMIT_RESET_MS_HEADER:
             return int(v) / 1000
-    raise ValueError(
-        f"response didn't contain {RATE_LIMIT_RESET_MS_HEADER} header")
+    raise ValueError(f"response didn't contain {RATE_LIMIT_RESET_MS_HEADER} header")
```

### Comparing `variational-0.4.1/LICENSE` & `variational-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `variational-0.4.1/README.md` & `variational-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `variational-0.4.1/pyproject.toml` & `variational-0.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "variational"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="Variational Research", email="hello@variational.io" },
 ]
 dependencies = [
     "requests >= 2.12",
     "Brotli >= 1.0",
     "eth-account >= 0.11"
```

### Comparing `variational-0.4.1/PKG-INFO` & `variational-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: variational
-Version: 0.4.1
+Version: 0.4.2
 Summary: Variational Reference SDK
 Project-URL: Homepage, https://variational.io
 Project-URL: Documentation, https://docs.variational.io/for-developers/api
 Project-URL: Repository, https://github.com/variational-research/variational-sdk-python/
 Project-URL: Issues, https://github.com/variational-research/variational-sdk-python/issues
 Author-email: Variational Research <hello@variational.io>
 License-File: LICENSE
```

