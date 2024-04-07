# Comparing `tmp/aiotgm-0.3.5.tar.gz` & `tmp/aiotgm-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotgm-0.3.5.tar", last modified: Thu Apr  4 10:59:30 2024, max compression
+gzip compressed data, was "aiotgm-0.3.6.tar", last modified: Sun Apr  7 09:37:35 2024, max compression
```

## Comparing `aiotgm-0.3.5.tar` & `aiotgm-0.3.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-04 10:59:30.914242 aiotgm-0.3.5/
--rw-r--r--   0 kali      (1000) root         (0)    35149 2023-12-11 13:46:43.000000 aiotgm-0.3.5/LICENSE
--rw-r--r--   0 kali      (1000) root         (0)    42090 2024-04-04 10:59:30.914242 aiotgm-0.3.5/PKG-INFO
--rw-r--r--   0 kali      (1000) root         (0)     1235 2024-04-04 07:17:27.000000 aiotgm-0.3.5/README.md
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-04 10:59:30.910242 aiotgm-0.3.5/aiotgm/
--rw-r--r--   0 kali      (1000) root         (0)      320 2024-04-04 10:59:04.000000 aiotgm-0.3.5/aiotgm/__init__.py
--rw-r--r--   0 kali      (1000) root         (0)    28031 2024-04-04 07:02:24.000000 aiotgm-0.3.5/aiotgm/api.py
--rw-r--r--   0 kali      (1000) root         (0)   283164 2024-04-04 07:07:39.000000 aiotgm-0.3.5/aiotgm/client.py
--rw-r--r--   0 kali      (1000) root         (0)     3123 2024-02-29 15:03:03.000000 aiotgm-0.3.5/aiotgm/constants.py
--rw-r--r--   0 kali      (1000) root         (0)      740 2024-04-01 12:33:00.000000 aiotgm-0.3.5/aiotgm/logging.py
--rw-r--r--   0 kali      (1000) root         (0)   311442 2024-04-04 10:55:59.000000 aiotgm-0.3.5/aiotgm/types.py
--rw-r--r--   0 kali      (1000) root         (0)     9152 2024-04-01 15:47:24.000000 aiotgm-0.3.5/aiotgm/update_manager.py
--rw-r--r--   0 kali      (1000) root         (0)      623 2024-03-17 17:13:52.000000 aiotgm-0.3.5/aiotgm/utils.py
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-04 10:59:30.910242 aiotgm-0.3.5/aiotgm.egg-info/
--rw-r--r--   0 kali      (1000) root         (0)    42090 2024-04-04 10:59:30.000000 aiotgm-0.3.5/aiotgm.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) root         (0)      348 2024-04-04 10:59:30.000000 aiotgm-0.3.5/aiotgm.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) root         (0)        1 2024-04-04 10:59:30.000000 aiotgm-0.3.5/aiotgm.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) root         (0)       48 2024-04-04 10:59:30.000000 aiotgm-0.3.5/aiotgm.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) root         (0)        7 2024-04-04 10:59:30.000000 aiotgm-0.3.5/aiotgm.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) root         (0)      441 2024-04-04 10:59:01.000000 aiotgm-0.3.5/pyproject.toml
--rw-r--r--   0 kali      (1000) root         (0)       38 2024-04-04 10:59:30.914242 aiotgm-0.3.5/setup.cfg
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-04 10:59:30.910242 aiotgm-0.3.5/tests/
--rw-r--r--   0 kali      (1000) root         (0)     1471 2024-03-14 20:26:02.000000 aiotgm-0.3.5/tests/test_func_ok.py
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-07 09:37:35.026950 aiotgm-0.3.6/
+-rw-r--r--   0 kali      (1000) root         (0)    35149 2023-12-11 13:46:43.000000 aiotgm-0.3.6/LICENSE
+-rw-r--r--   0 kali      (1000) root         (0)    42090 2024-04-07 09:37:35.026950 aiotgm-0.3.6/PKG-INFO
+-rw-r--r--   0 kali      (1000) root         (0)     1235 2024-04-04 07:17:27.000000 aiotgm-0.3.6/README.md
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-07 09:37:35.022949 aiotgm-0.3.6/aiotgm/
+-rw-r--r--   0 kali      (1000) root         (0)      320 2024-04-07 09:37:23.000000 aiotgm-0.3.6/aiotgm/__init__.py
+-rw-r--r--   0 kali      (1000) root         (0)    28031 2024-04-04 07:02:24.000000 aiotgm-0.3.6/aiotgm/api.py
+-rw-r--r--   0 kali      (1000) root         (0)   283164 2024-04-04 07:07:39.000000 aiotgm-0.3.6/aiotgm/client.py
+-rw-r--r--   0 kali      (1000) root         (0)     3123 2024-02-29 15:03:03.000000 aiotgm-0.3.6/aiotgm/constants.py
+-rw-r--r--   0 kali      (1000) root         (0)      740 2024-04-01 12:33:00.000000 aiotgm-0.3.6/aiotgm/logging.py
+-rw-r--r--   0 kali      (1000) root         (0)   381827 2024-04-07 09:35:26.000000 aiotgm-0.3.6/aiotgm/types.py
+-rw-r--r--   0 kali      (1000) root         (0)     9152 2024-04-01 15:47:24.000000 aiotgm-0.3.6/aiotgm/update_manager.py
+-rw-r--r--   0 kali      (1000) root         (0)      623 2024-03-17 17:13:52.000000 aiotgm-0.3.6/aiotgm/utils.py
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-07 09:37:35.026950 aiotgm-0.3.6/aiotgm.egg-info/
+-rw-r--r--   0 kali      (1000) root         (0)    42090 2024-04-07 09:37:35.000000 aiotgm-0.3.6/aiotgm.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) root         (0)      348 2024-04-07 09:37:35.000000 aiotgm-0.3.6/aiotgm.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) root         (0)        1 2024-04-07 09:37:35.000000 aiotgm-0.3.6/aiotgm.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) root         (0)       48 2024-04-07 09:37:35.000000 aiotgm-0.3.6/aiotgm.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) root         (0)        7 2024-04-07 09:37:35.000000 aiotgm-0.3.6/aiotgm.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) root         (0)      441 2024-04-07 09:37:21.000000 aiotgm-0.3.6/pyproject.toml
+-rw-r--r--   0 kali      (1000) root         (0)       38 2024-04-07 09:37:35.026950 aiotgm-0.3.6/setup.cfg
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-07 09:37:35.026950 aiotgm-0.3.6/tests/
+-rw-r--r--   0 kali      (1000) root         (0)     1471 2024-03-14 20:26:02.000000 aiotgm-0.3.6/tests/test_func_ok.py
```

### Comparing `aiotgm-0.3.5/LICENSE` & `aiotgm-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.5/PKG-INFO` & `aiotgm-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotgm
-Version: 0.3.5
+Version: 0.3.6
 Author: unixtux
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `aiotgm-0.3.5/README.md` & `aiotgm-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.5/aiotgm/api.py` & `aiotgm-0.3.6/aiotgm/api.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.5/aiotgm/client.py` & `aiotgm-0.3.6/aiotgm/client.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.5/aiotgm/constants.py` & `aiotgm-0.3.6/aiotgm/constants.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.5/aiotgm/logging.py` & `aiotgm-0.3.6/aiotgm/logging.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.5/aiotgm/types.py` & `aiotgm-0.3.6/aiotgm/types.py`

 * *Files 13% similar despite different names*

```diff
@@ -2039,14 +2039,20 @@
     This object contains information about the chat whose identifier was shared
     with the bot using a :obj:`~aiotgm.types.KeyboardButtonRequestChat` button.
 
     :param request_id: Identifier of the request.
     :type request_id: :obj:`int`
     :param chat_id: Identifier of the shared chat. This number may have more than 32 significant bits and some programming languages may have difficulty/silent defects in interpreting it. But it has at most 52 significant bits, so a 64-bit integer or double-precision float type are safe for storing this identifier. The bot may not have access to the chat and could be unable to use this identifier, unless the chat is already known to the bot by some other means.
     :type chat_id: :obj:`int`
+    :param title: Title of the chat, if the title was requested by the bot.
+    :type title: :obj:`str`, optional
+    :param username: Username of the chat, if the username was requested by the bot and available.
+    :type username: :obj:`str`, optional
+    :param photo: Available sizes of the chat photo, if the photo was requested by the bot.
+    :type photo: :obj:`list` of :obj:`~aiotgm.types.PhotoSize`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
         obj['request_id'] = res.get('request_id')
         obj['chat_id'] = res.get('chat_id')
@@ -3100,15 +3106,15 @@
 class InlineKeyboardMarkup(TelegramType):
     '''
     https://core.telegram.org/bots/api#inlinekeyboardmarkup
 
     This object represents an `inline keyboard <https://core.telegram.org/bots/features#inline-keyboards>`_ that appears right next to the message it belongs to.
 
     :param inline_keyboard: Array of button rows, each represented by an Array of :obj:`~aiotgm.types.InlineKeyboardButton` objects.
-    :type inline_keyboard: :obj:`list` of :obj:`list` of :obj:`~aiotgm.types.InlineKeyboardButton`
+    :type inline_keyboard: :obj:`list` of :obj:`list` of :obj:`~aiotgm.types.InlineKeyboardButton`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
         obj['inline_keyboard'] = [[InlineKeyboardButton._dese(kwargs) for kwargs in lst] for lst in res.get('inline_keyboard')]
         return cls(**obj)
@@ -4750,90 +4756,332 @@
         self.width = width
         self.height = height
         self.duration = duration
         self.supports_streaming = supports_streaming
         self.has_spoiler = has_spoiler
 
 
+class InputSticker(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#inputsticker
 
+    This object describes a sticker to be added to a sticker set.
+
+    :param sticker: The added sticker. Pass a file_id as a String to send a file that already exists on the Telegram servers, pass an HTTP URL as a String for Telegram to get a file from the Internet, upload a new one using multipart/form-data, or pass “attach://<file_attach_name>” to upload a new one using multipart/form-data under <file_attach_name> name. Animated and video stickers can't be uploaded via HTTP URL. `More information on Sending Files » <https://core.telegram.org/bots/api#sending-files>`_.
+    :type sticker: :obj:`~aiotgm.types.InputFile` or :obj:`str`
+    :param format: Format of the added sticker, must be one of “static” for a **.WEBP** or **.PNG** image, “animated” for a **.TGS** animation, “video” for a **WEBM** video.
+    :type format: :obj:`str`
+    :param emoji_list: List of 1-20 emoji associated with the sticker.
+    :type emoji_list: :obj:`list` of :obj:`str`
+    :param mask_position: Position where the mask should be placed on faces. For “mask” stickers only.
+    :type mask_position: :obj:`~aiotgm.types.MaskPosition`, optional
+    :param keywords: List of 0-20 search keywords for the sticker with total length of up to 64 characters. For “regular” and “custom_emoji” stickers only.
+    :type keywords: :obj:`list` of :obj:`str`, optional
+    '''
+    def __init__(
+        self,
+        sticker: Union[InputFile, str],
+        format: str,
+        emoji_list: list[str],
+        mask_position: Optional[MaskPosition] = None,
+        keywords: Optional[list[str]] = None
+    ):
+        self.sticker = sticker
+        self.format = format
+        self.emoji_list = emoji_list
+        self.mask_position = mask_position
+        self.keywords = keywords
 
 
+class InputTextMessageContent(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#inputtextmessagecontent
 
+    Represents the :obj:`content <aiotgm.types.InputMessageContent>`
+    of a text message to be sent as the result of an inline query.
 
+    :param message_text: Text of the message to be sent, 1-4096 characters.
+    :type message_text: :obj:`str`
+    :param parse_mode: Mode for parsing entities in the message text. See `formatting options <https://core.telegram.org/bots/api#formatting-options>`_ for more details.
+    :type parse_mode: :obj:`str`, optional
+    :param entities: List of special entities that appear in message text, which can be specified instead of *parse_mode*.
+    :type entities: :obj:`list` of :obj:`~aiotgm.types.MessageEntity`, optional
+    :param link_preview_options: Link preview generation options for the message.
+    :type link_preview_options: :obj:`~aiotgm.types.LinkPreviewOptions`, optional
+    '''
+    def __init__(
+        self,
+        message_text: str,
+        parse_mode: Optional[str] = None,
+        entities: Optional[list[MessageEntity]] = None,
+        link_preview_options: Optional[LinkPreviewOptions] = None
+    ):
+        self.message_text = message_text
+        self.parse_mode = parse_mode
+        self.entities = entities
+        self.link_preview_options = link_preview_options
 
 
-class SwitchInlineQueryChosenChat(TelegramType):
+class InputVenueMessageContent(TelegramType):
     '''
-    https://core.telegram.org/bots/api#switchinlinequerychosenchat
+    https://core.telegram.org/bots/api#inputvenuemessagecontent
 
-    This object represents an inline button that switches the current user
-    to inline mode in a chosen chat, with an optional default inline query.
+    Represents the :obj:`content <aiotgm.types.InputMessageContent>`
+    of a venue message to be sent as the result of an inline query.
+
+    :param latitude: Latitude of the venue in degrees.
+    :type latitude: :obj:`float`
+    :param longitude: Longitude of the venue in degrees.
+    :type longitude: :obj:`float`
+    :param title: Name of the venue.
+    :type title: :obj:`str`
+    :param address: Address of the venue.
+    :type address: :obj:`str`
+    :param foursquare_id: Foursquare identifier of the venue, if known.
+    :type foursquare_id: :obj:`str`, optional
+    :param foursquare_type: Foursquare type of the venue, if known. (For example, “arts_entertainment/default”, “arts_entertainment/aquarium” or “food/icecream”.)
+    :type foursquare_type: :obj:`str`, optional
+    :param google_place_id: Google Places identifier of the venue.
+    :type google_place_id: :obj:`str`, optional
+    :param google_place_type: Google Places type of the venue. (See `supported types <https://developers.google.com/places/web-service/supported_types>`_.)
+    :type google_place_type: :obj:`str`, optional
+    '''
+    def __init__(
+        self,
+        latitude: float,
+        longitude: float,
+        title: str,
+        address: str,
+        foursquare_id: Optional[str] = None,
+        foursquare_type: Optional[str] = None,
+        google_place_id: Optional[str] = None,
+        google_place_type: Optional[str] = None
+    ):
+        self.latitude = latitude
+        self.longitude = longitude
+        self.title = title
+        self.address = address
+        self.foursquare_id = foursquare_id
+        self.foursquare_type = foursquare_type
+        self.google_place_id = google_place_id
+        self.google_place_type = google_place_type
+
+
+class Invoice(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#invoice
+
+    This object contains basic information about an invoice.
+
+    :param title: Product name.
+    :type title: :obj:`str`
+    :param description: Product description.
+    :type description: :obj:`str`
+    :param start_parameter: Unique bot deep-linking parameter that can be used to generate this invoice.
+    :type start_parameter: :obj:`str`
+    :param currency: Three-letter ISO 4217 `currency <https://core.telegram.org/bots/payments#supported-currencies>`_ code.
+    :type currency: :obj:`str`
+    :param total_amount: Total price in the *smallest units* of the currency (integer, **not** float/double). For example, for a price of ``US$ 1.45`` pass ``amount = 145``. See the *exp* parameter in `currencies.json <https://core.telegram.org/bots/payments/currencies.json>`_, it shows the number of digits past the decimal point for each currency (2 for the majority of currencies).
+    :type total_amount: :obj:`int`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['query'] = res.get('query')
-        obj['allow_user_chats'] = res.get('allow_user_chats')
-        obj['allow_bot_chats'] = res.get('allow_bot_chats')
-        obj['allow_group_chats'] = res.get('allow_group_chats')
-        obj['allow_channel_chats'] = res.get('allow_channel_chats')
+        obj['title'] = res.get('title')
+        obj['description'] = res.get('description')
+        obj['start_parameter'] = res.get('start_parameter')
+        obj['currency'] = res.get('currency')
+        obj['total_amount'] = res.get('total_amount')
         return cls(**obj)
 
     def __init__(
         self,
-        query: Optional[str] = None,
-        allow_user_chats: Optional[bool] = None,
-        allow_bot_chats: Optional[bool] = None,
-        allow_group_chats: Optional[bool] = None,
-        allow_channel_chats: Optional[bool] = None
+        title: str,
+        description: str,
+        start_parameter: str,
+        currency: str,
+        total_amount: int
     ):
-        self.query = query
-        self.allow_user_chats = allow_user_chats
-        self.allow_bot_chats = allow_bot_chats
-        self.allow_group_chats = allow_group_chats
-        self.allow_channel_chats = allow_channel_chats
+        self.title = title
+        self.description = description
+        self.start_parameter = start_parameter
+        self.currency = currency
+        self.total_amount = total_amount
 
 
-class LoginUrl(TelegramType):
+class KeyboardButton(TelegramType):
     '''
-    https://core.telegram.org/bots/api#loginurl
+    https://core.telegram.org/bots/api#keyboardbutton
 
-    This object represents a parameter of the inline keyboard button used to automatically authorize
-    a user. Serves as a great replacement for the Telegram Login Widget when the user is coming from
-    Telegram. All the user needs to do is tap/click a button and confirm that they want to log in.
+    This object represents one button of the reply keyboard. For simple text buttons, :obj:`String` can be
+    used instead of this object to specify the button text. The optional fields *web_app*, *request_users*,
+    *request_chat*, *request_contact*, *request_location*, and *request_poll* are mutually exclusive.
+
+    :param text: Text of the button. If none of the optional fields are used, it will be sent as a message when the button is pressed.
+    :type text: :obj:`str`
+    :param request_users: If specified, pressing the button will open a list of suitable users. Identifiers of selected users will be sent to the bot in a “users_shared” service message. Available in private chats only.
+    :type request_users: :obj:`~aiotgm.types.KeyboardButtonRequestUsers`, optional
+    :param request_chat: If specified, pressing the button will open a list of suitable chats. Tapping on a chat will send its identifier to the bot in a “chat_shared” service message. Available in private chats only.
+    :type request_chat: :obj:`~aiotgm.types.KeyboardButtonRequestChat`, optional
+    :param request_contact: If :obj:`True`, the user's phone number will be sent as a contact when the button is pressed. Available in private chats only.
+    :type request_contact: :obj:`bool`, optional
+    :param request_location: If :obj:`True`, the user's current location will be sent when the button is pressed. Available in private chats only.
+    :type request_location: :obj:`bool`, optional
+    :param request_poll: If specified, the user will be asked to create a poll and send it to the bot when the button is pressed. Available in private chats only.
+    :type request_poll: :obj:`~aiotgm.types.KeyboardButtonPollType`, optional
+    :param web_app: If specified, the described `Web App <https://core.telegram.org/bots/webapps>`_ will be launched when the button is pressed. The Web App will be able to send a “web_app_data” service message. Available in private chats only.
+    :type web_app: :obj:`~aiotgm.types.WebAppInfo`, optional
     '''
-    @classmethod
-    @_parse_result
-    def _dese(cls, res: dict):
-        obj = {}
-        obj['url'] = res.get('url')
-        obj['forward_text'] = res.get('forward_text')
-        obj['bot_username'] = res.get('bot_username')
-        obj['request_write_access'] = res.get('request_write_access')
-        return cls(**obj)
+    def __init__(
+        self,
+        text: str,
+        request_users: Optional[KeyboardButtonRequestUsers] = None,
+        request_chat: Optional[KeyboardButtonRequestChat] = None,
+        request_contact: Optional[bool] = None,
+        request_location: Optional[bool] = None,
+        request_poll: Optional[KeyboardButtonPollType] = None,
+        web_app: Optional[WebAppInfo] = None
+    ):
+        self.text = text
+        self.request_users = request_users
+        self.request_chat = request_chat
+        self.request_contact = request_contact
+        self.request_location = request_location
+        self.request_poll = request_poll
+        self.web_app = web_app
 
+
+class KeyboardButtonPollType(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#keyboardbuttonpolltype
+
+    This object represents type of a poll, which is allowed to
+    be created and sent when the corresponding button is pressed.
+
+    :param type: If *quiz* is passed, the user will be allowed to create only polls in the quiz mode. If *regular* is passed, only regular polls will be allowed. Otherwise, the user will be allowed to create a poll of any type.
+    :type type: :obj:`str`, optional
+    '''
     def __init__(
         self,
-        url: str,
-        forward_text: Optional[str] = None,
-        bot_username: Optional[str] = None,
-        request_write_access: Optional[bool] = None
+        type: Optional[str] = None
     ):
-        self.url = url
-        self.forward_text = forward_text
-        self.bot_username = bot_username
-        self.request_write_access = request_write_access
+        self.type = type
+
+
+class KeyboardButtonRequestChat(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#keyboardbuttonrequestchat
+
+    This object defines the criteria used to request a suitable chat. Information about the
+    selected chat will be shared with the bot when the corresponding button is pressed. The bot
+    will be granted requested rights in the chat if appropriate `More about requesting chats » <https://core.telegram.org/bots/features#chat-and-user-selection>`_.
+
+    :param request_id: Signed 32-bit identifier of the request, which will be received back in the :obj:`~aiotgm.types.ChatShared` object. Must be unique within the message.
+    :type request_id: :obj:`int`
+    :param chat_is_channel: Pass :obj:`True` to request a channel chat, pass :obj:`False` to request a group or a supergroup chat.
+    :type chat_is_channel: :obj:`bool`
+    :param chat_is_forum: Pass :obj:`True` to request a forum supergroup, pass :obj:`False` to request a non-forum chat. If not specified, no additional restrictions are applied.
+    :type chat_is_forum: :obj:`bool`, optional
+    :param chat_has_username: Pass :obj:`True` to request a supergroup or a channel with a username, pass :obj:`False` to request a chat without a username. If not specified, no additional restrictions are applied.
+    :type chat_has_username: :obj:`bool`, optional
+    :param chat_is_created: Pass :obj:`True` to request a chat owned by the user. Otherwise, no additional restrictions are applied.
+    :type chat_is_created: :obj:`bool`, optional
+    :param user_administrator_rights: A JSON-serialized object listing the required administrator rights of the user in the chat. The rights must be a superset of *bot_administrator_rights*. If not specified, no additional restrictions are applied.
+    :type user_administrator_rights: :obj:`~aiotgm.types.ChatAdministratorRights`, optional
+    :param bot_administrator_rights: A JSON-serialized object listing the required administrator rights of the bot in the chat. The rights must be a subset of *user_administrator_rights*. If not specified, no additional restrictions are applied.
+    :type bot_administrator_rights: :obj:`~aiotgm.types.ChatAdministratorRights`, optional
+    :param bot_is_member: Pass :obj:`True` to request a chat with the bot as a member. Otherwise, no additional restrictions are applied.
+    :type bot_is_member: :obj:`bool`, optional
+    :param request_title: Pass :obj:`True` to request the chat's title.
+    :type request_title: :obj:`bool`, optional
+    :param request_username: Pass :obj:`True` to request the chat's username.
+    :type request_username: :obj:`bool`, optional
+    :param request_photo: Pass :obj:`True` to request the chat's photo.
+    :type request_photo: :obj:`bool`, optional
+    '''
+    def __init__(
+        self,
+        request_id: int,
+        chat_is_channel: bool,
+        chat_is_forum: Optional[bool] = None,
+        chat_has_username: Optional[bool] = None,
+        chat_is_created: Optional[bool] = None,
+        user_administrator_rights: Optional[ChatAdministratorRights] = None,
+        bot_administrator_rights: Optional[ChatAdministratorRights] = None,
+        bot_is_member: Optional[bool] = None,
+        request_title: Optional[bool] = None,
+        request_username: Optional[bool] = None,
+        request_photo: Optional[bool] = None
+    ):
+        self.request_id = request_id
+        self.chat_is_channel = chat_is_channel
+        self.chat_is_forum = chat_is_forum
+        self.chat_has_username = chat_has_username
+        self.chat_is_created = chat_is_created
+        self.user_administrator_rights = user_administrator_rights
+        self.bot_administrator_rights = bot_administrator_rights
+        self.bot_is_member = bot_is_member
+        self.request_title = request_title
+        self.request_username = request_username
+        self.request_photo = request_photo
+
+
+class KeyboardButtonRequestUsers(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#keyboardbuttonrequestusers
+
+    This object defines the criteria used to request suitable users. Information about the
+    selected users will be shared with the bot when the corresponding button is pressed.
+    `More about requesting users » <https://core.telegram.org/bots/features#chat-and-user-selection>`_.
+
+    :param request_id: Signed 32-bit identifier of the request that will be received back in the :obj:`~aiotgm.types.UsersShared` object. Must be unique within the message.
+    :type request_id: :obj:`int`
+    :param user_is_bot: Pass :obj:`True` to request bots, pass :obj:`False` to request regular users. If not specified, no additional restrictions are applied.
+    :type user_is_bot: :obj:`bool`, optional
+    :param user_is_premium: Pass :obj:`True` to request premium users, pass :obj:`False` to request non-premium users. If not specified, no additional restrictions are applied.
+    :type user_is_premium: :obj:`bool`, optional
+    :param max_quantity: The maximum number of users to be selected; 1-10. Defaults to :obj:`1`.
+    :type max_quantity: :obj:`int`, optional
+    :param request_name: Pass :obj:`True` to request the users' first and last name.
+    :type request_name: :obj:`bool`, optional
+    :param request_username: Pass :obj:`True` to request the users' username.
+    :type request_username: :obj:`bool`, optional
+    :param request_photo: Pass :obj:`True` to request the users' photo.
+    :type request_photo: :obj:`bool`, optional
+    '''
+    def __init__(
+        self,
+        request_id: int,
+        user_is_bot: Optional[bool] = None,
+        user_is_premium: Optional[bool] = None,
+        max_quantity: Optional[int] = None,
+        request_name: Optional[bool] = None,
+        request_username: Optional[bool] = None,
+        request_photo: Optional[bool] = None
+    ):
+        self.request_id = request_id
+        self.user_is_bot = user_is_bot
+        self.user_is_premium = user_is_premium
+        self.max_quantity = max_quantity
+        self.request_name = request_name
+        self.request_username = request_username
+        self.request_photo = request_photo
 
 
 class LabeledPrice(TelegramType):
     '''
     https://core.telegram.org/bots/api#labeledprice
 
     This object represents a portion of the price for goods or services.
+
+    :param label: Portion label.
+    :type label: :obj:`str`
+    :param amount: Price of the product in the *smallest units* of the `currency <https://core.telegram.org/bots/payments#supported-currencies>`_ (integer, **not** float/double). For example, for a price of ``US$ 1.45`` pass ``amount = 145``. See the *exp* parameter in `currencies.json <https://core.telegram.org/bots/payments/currencies.json>`_, it shows the number of digits past the decimal point for each currency (2 for the majority of currencies).
+    :type amount: :obj:`int`
     '''
     def __init__(
         self,
         label: str,
         amount: int
     ):
         self.label = label
@@ -4841,14 +5089,25 @@
 
 
 class LinkPreviewOptions(TelegramType):
     '''
     https://core.telegram.org/bots/api#linkpreviewoptions
 
     Describes the options used for link preview generation.
+
+    :param is_disabled: :obj:`True`, if the link preview is disabled.
+    :type is_disabled: :obj:`bool`, optional
+    :param url: URL to use for the link preview. If empty, then the first URL found in the message text will be used.
+    :type url: :obj:`str`, optional
+    :param prefer_small_media: :obj:`True`, if the media in the link preview is supposed to be shrunk; ignored if the URL isn't explicitly specified or media size change isn't supported for the preview.
+    :type prefer_small_media: :obj:`bool`, optional
+    :param prefer_large_media: :obj:`True`, if the media in the link preview is supposed to be enlarged; ignored if the URL isn't explicitly specified or media size change isn't supported for the preview.
+    :type prefer_large_media: :obj:`bool`, optional
+    :param show_above_text: :obj:`True`, if the link preview must be shown above the message text; otherwise, the link preview will be shown below the message text.
+    :type show_above_text: :obj:`bool`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
         obj['is_disabled'] = res.get('is_disabled')
         obj['url'] = res.get('url')
@@ -4868,166 +5127,374 @@
         self.is_disabled = is_disabled
         self.url = url
         self.prefer_small_media = prefer_small_media
         self.prefer_large_media = prefer_large_media
         self.show_above_text = show_above_text
 
 
-class User(TelegramType):
+class Location(TelegramType):
     '''
-    https://core.telegram.org/bots/api#user
+    https://core.telegram.org/bots/api#location
 
-    This object represents a Telegram user or bot.
+    This object represents a point on the map.
+
+    :param latitude: Latitude as defined by sender.
+    :type latitude: :obj:`float`
+    :param longitude: Longitude as defined by sender.
+    :type longitude: :obj:`float`
+    :param horizontal_accuracy: The radius of uncertainty for the location, measured in meters; 0-1500.
+    :type horizontal_accuracy: :obj:`float`, optional
+    :param live_period: Time relative to the message sending date, during which the location can be updated; in seconds. For active live locations only.
+    :type live_period: :obj:`int`, optional
+    :param heading: The direction in which user is moving, in degrees; 1-360. For active live locations only.
+    :type heading: :obj:`int`, optional
+    :param proximity_alert_radius: The maximum distance for proximity alerts about approaching another chat member, in meters. For sent live locations only.
+    :type proximity_alert_radius: :obj:`int`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['id'] = res.get('id')
-        obj['is_bot'] = res.get('is_bot')
-        obj['first_name'] = res.get('first_name')
-        obj['last_name'] = res.get('last_name')
-        obj['username'] = res.get('username')
-        obj['language_code'] = res.get('language_code')
-        obj['is_premium'] = res.get('is_premium')
-        obj['added_to_attachment_menu'] = res.get('added_to_attachment_menu')
-        obj['can_join_groups'] = res.get('can_join_groups')
-        obj['can_read_all_group_messages'] = res.get('can_read_all_group_messages')
-        obj['supports_inline_queries'] = res.get('supports_inline_queries')
-        obj['can_connect_to_business'] = res.get('can_connect_to_business')
+        obj['latitude'] = res.get('latitude')
+        obj['longitude'] = res.get('longitude')
+        obj['horizontal_accuracy'] = res.get('horizontal_accuracy')
+        obj['live_period'] = res.get('live_period')
+        obj['heading'] = res.get('heading')
+        obj['proximity_alert_radius'] = res.get('proximity_alert_radius')
         return cls(**obj)
 
     def __init__(
         self,
-        id: int,
-        is_bot: bool,
-        first_name: str,
-        last_name: Optional[str] = None,
-        username: Optional[str] = None,
-        language_code: Optional[str] = None,
-        is_premium: Optional[Literal[True]] = None,
-        added_to_attachment_menu: Optional[Literal[True]] = None,
-        can_join_groups: Optional[bool] = None,
-        can_read_all_group_messages: Optional[bool] = None,
-        supports_inline_queries: Optional[bool] = None,
-        can_connect_to_business: Optional[bool] = None
+        latitude: float,
+        longitude: float,
+        horizontal_accuracy: Optional[float] = None,
+        live_period: Optional[int] = None,
+        heading: Optional[int] = None,
+        proximity_alert_radius: Optional[int] = None
     ):
-        self.id = id
-        self.is_bot = is_bot
-        self.first_name = first_name
-        self.last_name = last_name
-        self.username = username
-        self.language_code = language_code
-        self.is_premium = is_premium
-        self.added_to_attachment_menu = added_to_attachment_menu
-        self.can_join_groups = can_join_groups
-        self.can_read_all_group_messages = can_read_all_group_messages
-        self.supports_inline_queries = supports_inline_queries
-        self.can_connect_to_business = can_connect_to_business
+        self.latitude = latitude
+        self.longitude = longitude
+        self.horizontal_accuracy = horizontal_accuracy
+        self.live_period = live_period
+        self.heading = heading
+        self.proximity_alert_radius = proximity_alert_radius
 
 
-class MessageEntity(TelegramType):
+class LoginUrl(TelegramType):
     '''
-    https://core.telegram.org/bots/api#messageentity
+    https://core.telegram.org/bots/api#loginurl
+
+    This object represents a parameter of the inline keyboard button used to automatically authorize
+    a user. Serves as a great replacement for the `Telegram Login Widget <https://core.telegram.org/widgets/login>`_
+    when the user is coming from Telegram. All the user needs to do is tap/click a button and confirm that they want to log in.
 
-    This object represents one special entity in a text message. For example, hashtags, usernames, URLs, etc.
+    Telegram apps support these buttons as of `version 5.7 <https://telegram.org/blog/privacy-discussions-web-bots#meet-seamless-web-bots>`_.
+
+        Sample bot: `@discussbot <https://t.me/discussbot>`_
+
+    :param url:
+        An HTTPS URL to be opened with user authorization data added to the query string when the button is pressed. If the user refuses to provide authorization data, the original URL without information about the user will be opened. The data added is the same as described in `Receiving authorization data <https://core.telegram.org/widgets/login#receiving-authorization-data>`_.
+
+        **NOTE**: You **must** always check the hash of the received data to verify the authentication and the integrity of the data as described in `Checking authorization <https://core.telegram.org/widgets/login#checking-authorization>`_.
+    :type url: :obj:`str`
+    :param forward_text: New text of the button in forwarded messages.
+    :type forward_text: :obj:`str`, optional
+    :param bot_username: Username of a bot, which will be used for user authorization. See `Setting up a bot <https://core.telegram.org/widgets/login#setting-up-a-bot>`_ for more details. If not specified, the current bot's username will be assumed. The url's domain must be the same as the domain linked with the bot. See `Linking your domain to the bot <https://core.telegram.org/widgets/login#linking-your-domain-to-the-bot>`_ for more details.
+    :type bot_username: :obj:`str`, optional
+    :param request_write_access: Pass :obj:`True` to request the permission for your bot to send messages to the user.
+    :type request_write_access: :obj:`bool`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['type'] = res.get('type')
-        obj['offset'] = res.get('offset')
-        obj['length'] = res.get('length')
         obj['url'] = res.get('url')
-        obj['user'] = User._dese(res.get('user'))
-        obj['language'] = res.get('language')
-        obj['custom_emoji_id'] = res.get('custom_emoji_id')
+        obj['forward_text'] = res.get('forward_text')
+        obj['bot_username'] = res.get('bot_username')
+        obj['request_write_access'] = res.get('request_write_access')
         return cls(**obj)
 
     def __init__(
         self,
-        type: str,
-        offset: int,
-        length: int,
-        url: Optional[str] = None,
-        user: Optional[User] = None,
-        language: Optional[str] = None,
-        custom_emoji_id: Optional[str] = None
+        url: str,
+        forward_text: Optional[str] = None,
+        bot_username: Optional[str] = None,
+        request_write_access: Optional[bool] = None
     ):
-        self.type = type
-        self.offset = offset
-        self.length = length
         self.url = url
-        self.user = user
-        self.language = language
-        self.custom_emoji_id = custom_emoji_id
+        self.forward_text = forward_text
+        self.bot_username = bot_username
+        self.request_write_access = request_write_access
 
 
-class TextQuote(TelegramType):
+class MaskPosition(TelegramType):
     '''
-    https://core.telegram.org/bots/api#textquote
+    https://core.telegram.org/bots/api#maskposition
 
-    This object contains information about the quoted part of a message that is replied to by the given message.
+    This object describes the position on faces where a mask should be placed by default.
+
+    :param point: The part of the face relative to which the mask should be placed. One of “forehead”, “eyes”, “mouth”, or “chin”.
+    :type point: :obj:`str`
+    :param x_shift: Shift by X-axis measured in widths of the mask scaled to the face size, from left to right. For example, choosing -1.0 will place mask just to the left of the default mask position.
+    :type x_shift: :obj:`float`
+    :param y_shift: Shift by Y-axis measured in heights of the mask scaled to the face size, from top to bottom. For example, 1.0 will place the mask just below the default mask position.
+    :type y_shift: :obj:`float`
+    :param scale: Mask scaling coefficient. For example, 2.0 means double size.
+    :type scale: :obj:`float`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['text'] = res.get('text')
-        obj['position'] = res.get('position')
-        obj['entities'] = [MessageEntity._dese(kwargs) for kwargs in res.get('entities')] if 'entities' in res else None
-        obj['is_manual'] = res.get('is_manual')
+        obj['point'] = res.get('point')
+        obj['x_shift'] = res.get('x_shift')
+        obj['y_shift'] = res.get('y_shift')
+        obj['scale'] = res.get('scale')
         return cls(**obj)
 
     def __init__(
         self,
-        text: str,
-        position: int,
-        entities: Optional[list[MessageEntity]] = None,
-        is_manual: Optional[Literal[True]] = None
+        point: str,
+        x_shift: float,
+        y_shift: float,
+        scale: float
     ):
-        self.text = text
-        self.position = position
-        self.entities = entities
-        self.is_manual = is_manual
+        self.point = point
+        self.x_shift = x_shift
+        self.y_shift = y_shift
+        self.scale = scale
 
 
-class ReplyParameters(TelegramType):
+class MenuButtonCommands(TelegramType):
     '''
-    https://core.telegram.org/bots/api#replyparameters
+    https://core.telegram.org/bots/api#menubuttoncommands
 
-    Describes reply parameters for the message that is being sent.
+    Represents a menu button, which opens the bot's list of commands.
+    '''
+    @classmethod
+    @_parse_result
+    def _dese(cls, res: dict):
+        obj = {}
+        return cls(**obj)
+
+    def __init__(self):
+        self.type = DEFAULT_MENU_BUTTON_COMMANDS
+
+
+class MenuButtonDefault(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#menubuttondefault
+
+    Describes that no specific value for the menu button was set.
+    '''
+    @classmethod
+    @_parse_result
+    def _dese(cls, res: dict):
+        obj = {}
+        return cls(**obj)
+
+    def __init__(self):
+        self.type = DEFAULT_MENU_BUTTON_DEFAULT
+
+
+class MenuButtonWebApp(TelegramType):
     '''
+    https://core.telegram.org/bots/api#menubuttonwebapp
+
+    Represents a menu button, which launches a `Web App <https://core.telegram.org/bots/webapps>`_.
+
+    :param text: Text on the button.
+    :type text: :obj:`str`
+    :param web_app: Description of the Web App that will be launched when the user presses the button. The Web App will be able to send an arbitrary message on behalf of the user using the method :meth:`~aiotgm.Client.answer_web_app_query`.
+    :type web_app: :obj:`~aiotgm.types.WebAppInfo`
+    '''
+    @classmethod
+    @_parse_result
+    def _dese(cls, res: dict):
+        obj = {}
+        obj['text'] = res.get('text')
+        obj['web_app'] = WebAppInfo._dese(res.get('web_app'))
+        return cls(**obj)
+
     def __init__(
         self,
-        message_id: int,
-        chat_id: Optional[Union[int, str]] = None,
-        allow_sending_without_reply: Optional[bool] = None,
-        quote: Optional[str] = None,
-        quote_parse_mode: Optional[str] = None,
-        quote_entities: Optional[list[MessageEntity]] = None,
-        quote_position: Optional[int] = None
+        text: str,
+        web_app: WebAppInfo
     ):
-        self.message_id = message_id
-        self.chat_id = chat_id
-        self.allow_sending_without_reply = allow_sending_without_reply
-        self.quote = quote
-        self.quote_parse_mode = quote_parse_mode
-        self.quote_entities = quote_entities
-        self.quote_position = quote_position
-
+        self.type = DEFAULT_MENU_BUTTON_WEB_APP
+        self.text = text
+        self.web_app = web_app
 
-# MaybeInaccessibleMessage: 2 SUBCLASSES ~~~~~~~~~~~~~~~~~
 
 class Message(TelegramType):
     '''
     https://core.telegram.org/bots/api#message
 
     This object represents a message.
+
+    :param message_id: Unique message identifier inside this chat.
+    :type message_id: :obj:`int`
+    :param date: Date the message was sent in Unix time. It is always a positive number, representing a valid date.
+    :type date: :obj:`int`
+    :param chat: Chat the message belongs to.
+    :type chat: :obj:`~aiotgm.types.Chat`
+    :param message_thread_id: Unique identifier of a message thread to which the message belongs; for supergroups only.
+    :type message_thread_id: :obj:`int`, optional
+    :param from_user: Sender of the message; empty for messages sent to channels. For backward compatibility, the field contains a fake sender user in non-channel chats, if the message was sent on behalf of a chat.
+    :type from_user: :obj:`~aiotgm.types.User`, optional
+    :param sender_chat: Sender of the message, sent on behalf of a chat. For example, the channel itself for channel posts, the supergroup itself for messages from anonymous group administrators, the linked channel for messages automatically forwarded to the discussion group. For backward compatibility, the field from contains a fake sender user in non-channel chats, if the message was sent on behalf of a chat.
+    :type sender_chat: :obj:`~aiotgm.types.Chat`, optional
+    :param sender_boost_count: If the sender of the message boosted the chat, the number of boosts added by the user.
+    :type sender_boost_count: :obj:`int`, optional
+    :param sender_business_bot: The bot that actually sent the message on behalf of the business account. Available only for outgoing messages sent on behalf of the connected business account.
+    :type sender_business_bot: :obj:`~aiotgm.types.User`, optional
+    :param business_connection_id: Unique identifier of the business connection from which the message was received. If non-empty, the message belongs to a chat of the corresponding business account that is independent from any potential bot chat which might share the same identifier.
+    :type business_connection_id: :obj:`str`, optional
+    :param forward_origin: Information about the original message for forwarded messages.
+    :type forward_origin: :obj:`~aiotgm.types.MessageOrigin`, optional
+    :param is_topic_message: :obj:`True`, if the message is sent to a forum topic.
+    :type is_topic_message: :obj:`True`, optional
+    :param is_automatic_forward: :obj:`True`, if the message is a channel post that was automatically forwarded to the connected discussion group.
+    :type is_automatic_forward: :obj:`True`, optional
+    :param reply_to_message: For replies in the same chat and message thread, the original message. Note that the Message object in this field will not contain further *reply_to_message* fields even if it itself is a reply.
+    :type reply_to_message: :obj:`~aiotgm.types.Message`, optional
+    :param external_reply: Information about the message that is being replied to, which may come from another chat or forum topic.
+    :type external_reply: :obj:`~aiotgm.types.ExternalReplyInfo`, optional
+    :param quote: For replies that quote part of the original message, the quoted part of the message.
+    :type quote: :obj:`~aiotgm.types.TextQuote`, optional
+    :param reply_to_story: For replies to a story, the original story.
+    :type reply_to_story: :obj:`~aiotgm.types.Story`, optional
+    :param via_bot: Bot through which the message was sent.
+    :type via_bot: :obj:`~aiotgm.types.User`, optional
+    :param edit_date: Date the message was last edited in Unix time.
+    :type edit_date: :obj:`int`, optional
+    :param has_protected_content: :obj:`True`, if the message can't be forwarded.
+    :type has_protected_content: :obj:`True`, optional
+    :param is_from_offline: :obj:`True`, if the message was sent by an implicit action, for example, as an away or a greeting business message, or as a scheduled message.
+    :type is_from_offline: :obj:`True`, optional
+    :param media_group_id: The unique identifier of a media message group this message belongs to.
+    :type media_group_id: :obj:`str`, optional
+    :param author_signature: Signature of the post author for messages in channels, or the custom title of an anonymous group administrator.
+    :type author_signature: :obj:`str`, optional
+    :param text: For text messages, the actual UTF-8 text of the message.
+    :type text: :obj:`str`, optional
+    :param entities: For text messages, special entities like usernames, URLs, bot commands, etc. that appear in the text.
+    :type entities: :obj:`list` of :obj:`~aiotgm.types.MessageEntity`, optional
+    :param link_preview_options: Options used for link preview generation for the message, if it is a text message and link preview options were changed.
+    :type link_preview_options: :obj:`~aiotgm.types.LinkPreviewOptions`, optional
+    :param animation: Message is an animation, information about the animation. For backward compatibility, when this field is set, the document field will also be set.
+    :type animation: :obj:`~aiotgm.types.Animation`, optional
+    :param audio: Message is an audio file, information about the file.
+    :type audio: :obj:`~aiotgm.types.Audio`, optional
+    :param document: Message is a general file, information about the file.
+    :type document: :obj:`~aiotgm.types.Document`, optional
+    :param photo: Message is a photo, available sizes of the photo.
+    :type photo: :obj:`list` of :obj:`~aiotgm.types.PhotoSize`, optional
+    :param sticker: Message is a sticker, information about the sticker.
+    :type sticker: :obj:`~aiotgm.types.Sticker`, optional
+    :param story: Message is a forwarded story.
+    :type story: :obj:`~aiotgm.types.Story`, optional
+    :param video: Message is a video, information about the video.
+    :type video: :obj:`~aiotgm.types.Video`, optional
+    :param video_note: Message is a `video note <https://telegram.org/blog/video-messages-and-telescope>`_, information about the video message.
+    :type video_note: :obj:`~aiotgm.types.VideoNote`, optional
+    :param voice: Message is a voice message, information about the file.
+    :type voice: :obj:`~aiotgm.types.Voice`, optional
+    :param caption: Caption for the animation, audio, document, photo, video or voice.
+    :type caption: :obj:`str`, optional
+    :param caption_entities: For messages with a caption, special entities like usernames, URLs, bot commands, etc. that appear in the caption.
+    :type caption_entities: :obj:`list` of :obj:`MessageEntity`, optional
+    :param has_media_spoiler: :obj:`True`, if the message media is covered by a spoiler animation.
+    :type has_media_spoiler: :obj:`True`, optional
+    :param contact: Message is a shared contact, information about the contact.
+    :type contact: :obj:`~aiotgm.types.Contact`, optional
+    :param dice: Message is a dice with random value.
+    :type dice: :obj:`~aiotgm.types.Dice`, optional
+    :param game: Message is a game, information about the game. `More about games » <https://core.telegram.org/bots/api#games>`_.
+    :type game: :obj:`~aiotgm.types.Game`, optional
+    :param poll: Message is a native poll, information about the poll.
+    :type poll: :obj:`~aiotgm.types.Poll`, optional
+    :param venue: Message is a venue, information about the venue. For backward compatibility, when this field is set, the location field will also be set.
+    :type venue: :obj:`~aiotgm.types.Venue`, optional
+    :param location: Message is a shared location, information about the location.
+    :type location: :obj:`~aiotgm.types.Location`, optional
+    :param new_chat_members: New members that were added to the group or supergroup and information about them (the bot itself may be one of these members).
+    :type new_chat_members: :obj:`list` of :obj:`~aiotgm.types.User`, optional
+    :param left_chat_member: A member was removed from the group, information about them (this member may be the bot itself).
+    :type left_chat_member: :obj:`~aiotgm.types.User`, optional
+    :param new_chat_title: A chat title was changed to this value.
+    :type new_chat_title: :obj:`str`, optional
+    :param new_chat_photo: A chat photo was change to this value.
+    :type new_chat_photo: :obj:`list` of :obj:`~aiotgm.types.PhotoSize`, optional
+    :param delete_chat_photo: Service message: the chat photo was deleted.
+    :type delete_chat_photo: :obj:`True`, optional
+    :param group_chat_created: Service message: the group has been created.
+    :type group_chat_created: :obj:`True`, optional
+    :param supergroup_chat_created: Service message: the supergroup has been created. This field can't be received in a message coming through updates, because bot can't be a member of a supergroup when it is created. It can only be found in reply_to_message if someone replies to a very first message in a directly created supergroup.
+    :type supergroup_chat_created: :obj:`True`, optional
+    :param channel_chat_created: Service message: the channel has been created. This field can't be received in a message coming through updates, because bot can't be a member of a channel when it is created. It can only be found in reply_to_message if someone replies to a very first message in a channel.
+    :type channel_chat_created: :obj:`True`, optional
+    :param message_auto_delete_timer_changed: Service message: auto-delete timer settings changed in the chat.
+    :type message_auto_delete_timer_changed: :obj:`~aiotgm.types.MessageAutoDeleteTimerChanged`, optional
+    :param migrate_to_chat_id: The group has been migrated to a supergroup with the specified identifier. This number may have more than 32 significant bits and some programming languages may have difficulty/silent defects in interpreting it. But it has at most 52 significant bits, so a signed 64-bit integer or double-precision float type are safe for storing this identifier.
+    :type migrate_to_chat_id: :obj:`int`, optional
+    :param migrate_from_chat_id: The supergroup has been migrated from a group with the specified identifier. This number may have more than 32 significant bits and some programming languages may have difficulty/silent defects in interpreting it. But it has at most 52 significant bits, so a signed 64-bit integer or double-precision float type are safe for storing this identifier.
+    :type migrate_from_chat_id: :obj:`int`, optional
+    :param pinned_message: Specified message was pinned. Note that the Message object in this field will not contain further *reply_to_message* fields even if it itself is a reply.
+    :type pinned_message: :obj:`~aiotgm.types.MaybeInaccessibleMessage`, optional
+    :param invoice: Message is an invoice for a `payment <https://core.telegram.org/bots/api#payments>`_, information about the invoice. `More about payments » <https://core.telegram.org/bots/api#payments>`_.
+    :type invoice: :obj:`~aiotgm.types.Invoice`, optional
+    :param successful_payment: Message is a service message about a successful payment, information about the payment. `More about payments » <https://core.telegram.org/bots/api#payments>`_.
+    :type successful_payment: :obj:`~aiotgm.types.SuccessfulPayment`, optional
+    :param users_shared: Service message: users were shared with the bot.
+    :type users_shared: :obj:`~aiotgm.types.UsersShared`, optional
+    :param chat_shared: Service message: a chat was shared with the bot.
+    :type chat_shared: :obj:`~aiotgm.types.ChatShared`, optional
+    :param connected_website: The domain name of the website on which the user has logged in. `More about Telegram Login » <https://core.telegram.org/widgets/login>`_.
+    :type connected_website: :obj:`str`, optional
+    :param write_access_allowed: Service message: the user allowed the bot to write messages after adding it to the attachment or side menu, launching a Web App from a link, or accepting an explicit request from a Web App sent by the method `requestWriteAccess <https://core.telegram.org/bots/webapps#initializing-mini-apps>`_.
+    :type write_access_allowed: :obj:`~aiotgm.types.WriteAccessAllowed`, optional
+    :param passport_data: Telegram Passport data.
+    :type passport_data: :obj:`~aiotgm.types.PassportData`, optional
+    :param proximity_alert_triggered: Service message. A user in the chat triggered another user's proximity alert while sharing Live Location.
+    :type proximity_alert_triggered: :obj:`~aiotgm.types.ProximityAlertTriggered`, optional
+    :param boost_added: Service message: user boosted the chat.
+    :type boost_added: :obj:`~aiotgm.types.ChatBoostAdded`, optional
+    :param forum_topic_created: Service message: forum topic created.
+    :type forum_topic_created: :obj:`~aiotgm.types.ForumTopicCreated`, optional
+    :param forum_topic_edited: Service message: forum topic edited.
+    :type forum_topic_edited: :obj:`~aiotgm.types.ForumTopicEdited`, optional
+    :param forum_topic_closed: Service message: forum topic closed.
+    :type forum_topic_closed: :obj:`~aiotgm.types.ForumTopicClosed`, optional
+    :param forum_topic_reopened: Service message: forum topic reopened.
+    :type forum_topic_reopened: :obj:`~aiotgm.types.ForumTopicReopened`, optional
+    :param general_forum_topic_hidden: Service message: the 'General' forum topic hidden.
+    :type general_forum_topic_hidden: :obj:`~aiotgm.types.GeneralForumTopicHidden`, optional
+    :param general_forum_topic_unhidden: Service message: the 'General' forum topic unhidden.
+    :type general_forum_topic_unhidden: :obj:`~aiotgm.types.GeneralForumTopicUnhidden`, optional
+    :param giveaway_created: Service message: a scheduled giveaway was created.
+    :type giveaway_created: :obj:`~aiotgm.types.GiveawayCreated`, optional
+    :param giveaway: The message is a scheduled giveaway message.
+    :type giveaway: :obj:`~aiotgm.types.Giveaway`, optional
+    :param giveaway_winners: A giveaway with public winners was completed.
+    :type giveaway_winners: :obj:`~aiotgm.types.GiveawayWinners`, optional
+    :param giveaway_completed: Service message: a giveaway without public winners was completed.
+    :type giveaway_completed: :obj:`~aiotgm.types.GiveawayCompleted`, optional
+    :param video_chat_scheduled: Service message: video chat scheduled.
+    :type video_chat_scheduled: :obj:`~aiotgm.types.VideoChatScheduled`, optional
+    :param video_chat_started: Service message: video chat started.
+    :type video_chat_started: :obj:`~aiotgm.types.VideoChatStarted`, optional
+    :param video_chat_ended: Service message: video chat ended.
+    :type video_chat_ended: :obj:`~aiotgm.types.VideoChatEnded`, optional
+    :param video_chat_participants_invited: Service message: new participants invited to a video chat.
+    :type video_chat_participants_invited: :obj:`~aiotgm.types.VideoChatParticipantsInvited`, optional
+    :param web_app_data: Service message: data sent by a Web App.
+    :type web_app_data: :obj:`~aiotgm.types.WebAppData`, optional
+    :param reply_markup: Inline keyboard attached to the message. ``login_url`` buttons are represented as ordinary ``url`` buttons.
+    :type reply_markup: :obj:`~aiotgm.types.InlineKeyboardMarkup`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
         obj['message_id'] = res.get('message_id')
         obj['date'] = res.get('date')
@@ -5272,221 +5739,259 @@
         self.video_chat_started = video_chat_started
         self.video_chat_ended = video_chat_ended
         self.video_chat_participants_invited = video_chat_participants_invited
         self.web_app_data = web_app_data
         self.reply_markup = reply_markup
 
 
-MaybeInaccessibleMessage = Union[Message, InaccessibleMessage]
-'''
-https://core.telegram.org/bots/api#maybeinaccessiblemessage
-
-This object describes a message that can be inaccessible to the bot.
-
-It can be one of:
+class MessageAutoDeleteTimerChanged(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#messageautodeletetimerchanged
 
-- Message
-- InaccessibleMessage
-'''
+    This object represents a service message about a change in auto-delete timer settings.
 
-def _dese_maybe_inaccessible_message(res: Optional[dict], /) -> Optional[MaybeInaccessibleMessage]:
-    '''
-    Function to deserialize MaybeInaccessibleMessage.
+    :param message_auto_delete_time: New auto-delete time for messages in the chat; in seconds.
+    :type message_auto_delete_time: :obj:`int`
     '''
-    if res is None: return None
-    obj = _check_dict(res)
-
-    if obj['date'] == 0:
-        return InaccessibleMessage._dese(obj, check_dict=False)
-    else:
-        return Message._dese(obj, check_dict=False)
+    @classmethod
+    @_parse_result
+    def _dese(cls, res: dict):
+        obj = {}
+        obj['message_auto_delete_time'] = res.get('message_auto_delete_time')
+        return cls(**obj)
 
-# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+    def __init__(
+        self,
+        message_auto_delete_time: int
+    ):
+        self.message_auto_delete_time = message_auto_delete_time
 
 
-class Location(TelegramType):
+class MessageEntity(TelegramType):
     '''
-    https://core.telegram.org/bots/api#location
+    https://core.telegram.org/bots/api#messageentity
 
-    This object represents a point on the map.
+    This object represents one special entity in a text message.
+    For example, hashtags, usernames, URLs, etc.
+
+    :param type: Type of the entity. Currently, can be “mention” (``@username``), “hashtag” (``#hashtag``), “cashtag” (``$USD``), “bot_command” (``/start@jobs_bot``), “url” (``https://telegram.org``), “email” (``do-not-reply@telegram.org``), “phone_number” (``+1-212-555-0123``), “bold” (**bold text**), “italic” (*italic text*), “underline” (underlined text), “strikethrough” (strikethrough text), “spoiler” (spoiler message), “blockquote” (block quotation), “code” (monowidth string), “pre” (monowidth block), “text_link” (for clickable text URLs), “text_mention” (for users `without usernames <https://telegram.org/blog/edit#new-mentions>`_), “custom_emoji” (for inline custom emoji stickers).
+    :type type: :obj:`str`
+    :param offset: Offset in `UTF-16 code units <https://core.telegram.org/api/entities#entity-length>`_ to the start of the entity.
+    :type offset: :obj:`int`
+    :param length: Length of the entity in `UTF-16 code units <https://core.telegram.org/api/entities#entity-length>`_.
+    :type length: :obj:`int`
+    :param url: For “text_link” only, URL that will be opened after user taps on the text.
+    :type url: :obj:`str`, optional
+    :param user: For “text_mention” only, the mentioned user.
+    :type user: :obj:`~aiotgm.types.User`, optional
+    :param language: For “pre” only, the programming language of the entity text.
+    :type language: :obj:`str`, optional
+    :param custom_emoji_id: For “custom_emoji” only, unique identifier of the custom emoji. Use :meth:`~aiotgm.Client.get_custom_emoji_stickers` to get full information about the sticker.
+    :type custom_emoji_id: :obj:`str`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['longitude'] = res.get('longitude')
-        obj['latitude'] = res.get('latitude')
-        obj['horizontal_accuracy'] = res.get('horizontal_accuracy')
-        obj['live_period'] = res.get('live_period')
-        obj['heading'] = res.get('heading')
-        obj['proximity_alert_radius'] = res.get('proximity_alert_radius')
+        obj['type'] = res.get('type')
+        obj['offset'] = res.get('offset')
+        obj['length'] = res.get('length')
+        obj['url'] = res.get('url')
+        obj['user'] = User._dese(res.get('user'))
+        obj['language'] = res.get('language')
+        obj['custom_emoji_id'] = res.get('custom_emoji_id')
         return cls(**obj)
 
     def __init__(
         self,
-        longitude: float,
-        latitude: float,
-        horizontal_accuracy: Optional[float] = None,
-        live_period: Optional[int] = None,
-        heading: Optional[int] = None,
-        proximity_alert_radius: Optional[int] = None
+        type: str,
+        offset: int,
+        length: int,
+        url: Optional[str] = None,
+        user: Optional[User] = None,
+        language: Optional[str] = None,
+        custom_emoji_id: Optional[str] = None
     ):
-        self.longitude = longitude
-        self.latitude = latitude
-        self.horizontal_accuracy = horizontal_accuracy
-        self.live_period = live_period
-        self.heading = heading
-        self.proximity_alert_radius = proximity_alert_radius
-
+        self.type = type
+        self.offset = offset
+        self.length = length
+        self.url = url
+        self.user = user
+        self.language = language
+        self.custom_emoji_id = custom_emoji_id
 
-# ReactionType: 2 SUBCLASSES ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-class ReactionTypeEmoji(TelegramType):
+class MessageId(TelegramType):
     '''
-    https://core.telegram.org/bots/api#reactiontypeemoji
+    https://core.telegram.org/bots/api#messageid
 
-    The reaction is based on an emoji.
+    This object represents a unique message identifier.
+
+    :param message_id: Unique message identifier.
+    :type message_id: :obj:`int`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['emoji'] = res.get('emoji')
+        obj['message_id'] = res.get('message_id')
         return cls(**obj)
 
     def __init__(
         self,
-        emoji: str
+        message_id: int
     ):
-        self.type = DEFAULT_REACTION_TYPE_EMOJI
-        self.emoji = emoji
+        self.message_id = message_id
 
 
-class ReactionTypeCustomEmoji(TelegramType):
+class MessageOriginChannel(TelegramType):
     '''
-    https://core.telegram.org/bots/api#reactiontypecustomemoji
+    https://core.telegram.org/bots/api#messageoriginchannel
 
-    The reaction is based on a custom emoji.
+    The message was originally sent to a channel chat.
+
+    :param date: Date the message was sent originally in Unix time.
+    :type date: :obj:`int`
+    :param chat: Channel chat to which the message was originally sent.
+    :type chat: :obj:`~aiotgm.types.Chat`
+    :param message_id: Unique message identifier inside the chat.
+    :type message_id: :obj:`int`
+    :param author_signature: Signature of the original post author.
+    :type author_signature: :obj:`str`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['custom_emoji_id'] = res.get('custom_emoji_id')
+        obj['date'] = res.get('date')
+        obj['chat'] = Chat._dese(res.get('chat'))
+        obj['message_id'] = res.get('message_id')
+        obj['author_signature'] = res.get('author_signature')
         return cls(**obj)
 
     def __init__(
         self,
-        custom_emoji_id: str
+        date: int,
+        chat: Chat,
+        message_id: int,
+        author_signature: Optional[str] = None
     ):
-        self.type = DEFAULT_REACTION_TYPE_CUSTOM_EMOJI
-        self.custom_emoji_id = custom_emoji_id
-
-
-ReactionType = Union[ReactionTypeEmoji, ReactionTypeCustomEmoji]
-'''
-https://core.telegram.org/bots/api#reactiontype
-
-This object describes the type of a reaction.
-
-Currently, it can be one of:
+        self.type = DEFAULT_MESSAGE_ORIGIN_CHANNEL
+        self.date = date
+        self.chat = chat
+        self.message_id = message_id
+        self.author_signature = author_signature
 
-- ReactionTypeEmoji
-- ReactionTypeCustomEmoji
-'''
 
-def _dese_reaction_type(res: Optional[dict], /) -> Optional[ReactionType]:
-    '''
-    Function to deserialize ReactionType.
+class MessageOriginChat(TelegramType):
     '''
-    if res is None: return None
-    obj = _check_dict(res)
-
-    type = obj.pop('type')
+    https://core.telegram.org/bots/api#messageoriginchat
 
-    if type == DEFAULT_REACTION_TYPE_EMOJI:
-        return ReactionTypeEmoji._dese(obj, check_dict=False)
+    The message was originally sent on behalf of a chat to a group chat.
 
-    elif type == DEFAULT_REACTION_TYPE_CUSTOM_EMOJI:
-        return ReactionTypeCustomEmoji._dese(obj, check_dict=False)
-    else:
-        raise ValueError(
-            'An error occurred during the deserialization'
-            f' of the type ReactionType. Invalid type: {type!r}.'
-        )
+    :param date: Date the message was sent originally in Unix time.
+    :type date: :obj:`int`
+    :param sender_chat: Chat that sent the message originally.
+    :type sender_chat: :obj:`~aiotgm.types.Chat`
+    :param author_signature: For messages originally sent by an anonymous chat administrator, original message author signature.
+    :type author_signature: :obj:`str`, optional
+    '''
+    @classmethod
+    @_parse_result
+    def _dese(cls, res: dict):
+        obj = {}
+        obj['date'] = res.get('date')
+        obj['sender_chat'] = Chat._dese(res.get('sender_chat'))
+        obj['author_signature'] = res.get('author_signature')
+        return cls(**obj)
 
-# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+    def __init__(
+        self,
+        date: int,
+        sender_chat: Chat,
+        author_signature: Optional[str] = None
+    ):
+        self.type = DEFAULT_MESSAGE_ORIGIN_CHAT
+        self.date = date
+        self.sender_chat = sender_chat
+        self.author_signature = author_signature
 
 
-class MessageReactionUpdated(TelegramType):
+class MessageOriginHiddenUser(TelegramType):
     '''
-    https://core.telegram.org/bots/api#messagereactionupdated
+    https://core.telegram.org/bots/api#messageoriginhiddenuser
 
-    This object represents a change of a reaction on a message performed by a user.
+    The message was originally sent by an unknown user.
+
+    :param date: Date the message was sent originally in Unix time.
+    :type date: :obj:`int`
+    :param sender_user_name: Name of the user that sent the message originally.
+    :type sender_user_name: :obj:`str`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['chat'] = Chat._dese(res.get('chat'))
-        obj['message_id'] = res.get('message_id')
         obj['date'] = res.get('date')
-        obj['old_reaction'] = [_dese_reaction_type(kwargs) for kwargs in res.get('old_reaction')]
-        obj['new_reaction'] = [_dese_reaction_type(kwargs) for kwargs in res.get('new_reaction')]
-        obj['user'] = User._dese(res.get('user'))
-        obj['actor_chat'] = Chat._dese(res.get('actor_chat'))
+        obj['sender_user_name'] = res.get('sender_user_name')
         return cls(**obj)
 
     def __init__(
         self,
-        chat: Chat,
-        message_id: int,
         date: int,
-        old_reaction: list[ReactionType],
-        new_reaction: list[ReactionType],
-        user: Optional[User] = None,
-        actor_chat: Optional[Chat] = None
+        sender_user_name: str
     ):
-        self.chat = chat
-        self.message_id = message_id
+        self.type = DEFAULT_MESSAGE_ORIGIN_HIDDEN_USER
         self.date = date
-        self.old_reaction = old_reaction
-        self.new_reaction = new_reaction
-        self.user = user
-        self.actor_chat = actor_chat
+        self.sender_user_name = sender_user_name
 
 
-class ReactionCount(TelegramType):
+class MessageOriginUser(TelegramType):
     '''
-    https://core.telegram.org/bots/api#reactioncount
+    https://core.telegram.org/bots/api#messageoriginuser
 
-    Represents a reaction added to a message along with the number of times it was added.
+    The message was originally sent by a known user.
+
+    :param date: Date the message was sent originally in Unix time.
+    :type date: :obj:`int`
+    :param sender_user: User that sent the message originally.
+    :type sender_user: :obj:`~aiotgm.types.User`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['type'] = _dese_reaction_type(res.get('type'))
-        obj['total_count'] = res.get('total_count')
+        obj['date'] = res.get('date')
+        obj['sender_user'] = User._dese(res.get('sender_user'))
         return cls(**obj)
 
     def __init__(
         self,
-        type: ReactionType,
-        total_count: int
+        date: int,
+        sender_user: User
     ):
-        self.type = type
-        self.total_count = total_count
+        self.type = DEFAULT_MESSAGE_ORIGIN_USER
+        self.date = date
+        self.sender_user = sender_user
 
 
 class MessageReactionCountUpdated(TelegramType):
     '''
     https://core.telegram.org/bots/api#messagereactioncountupdated
 
     This object represents reaction changes on a message with anonymous reactions.
+
+    :param chat: The chat containing the message.
+    :type chat: :obj:`~aiotgm.types.Chat`
+    :param message_id: Unique message identifier inside the chat.
+    :type message_id: :obj:`int`
+    :param date: Date of the change in Unix time.
+    :type date: :obj:`int`
+    :param reactions: List of reactions that are present on the message.
+    :type reactions: :obj:`list` of :obj:`~aiotgm.types.ReactionCount`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
         obj['chat'] = Chat._dese(res.get('chat'))
         obj['message_id'] = res.get('message_id')
@@ -5503,257 +6008,486 @@
     ):
         self.chat = chat
         self.message_id = message_id
         self.date = date
         self.reactions = reactions
 
 
-class MessageId(TelegramType):
+class MessageReactionUpdated(TelegramType):
     '''
-    https://core.telegram.org/bots/api#messageid
+    https://core.telegram.org/bots/api#messagereactionupdated
 
-    This object represents a unique message identifier.
+    This object represents a change of a reaction on a message performed by a user.
+
+    :param chat: The chat containing the message the user reacted to.
+    :type chat: :obj:`~aiotgm.types.Chat`
+    :param message_id: Unique identifier of the message inside the chat.
+    :type message_id: :obj:`int`
+    :param date: Date of the change in Unix time.
+    :type date: :obj:`int`
+    :param old_reaction: Previous list of reaction types that were set by the user.
+    :type old_reaction: :obj:`list` of :obj:`~aiotgm.types.ReactionType`
+    :param new_reaction: New list of reaction types that have been set by the user.
+    :type new_reaction: :obj:`list` of :obj:`~aiotgm.types.ReactionType`
+    :param user: The user that changed the reaction, if the user isn't anonymous.
+    :type user: :obj:`~aiotgm.types.User`, optional
+    :param actor_chat: The chat on behalf of which the reaction was changed, if the user is anonymous.
+    :type actor_chat: :obj:`~aiotgm.types.Chat`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
+        obj['chat'] = Chat._dese(res.get('chat'))
         obj['message_id'] = res.get('message_id')
+        obj['date'] = res.get('date')
+        obj['old_reaction'] = [_dese_reaction_type(kwargs) for kwargs in res.get('old_reaction')]
+        obj['new_reaction'] = [_dese_reaction_type(kwargs) for kwargs in res.get('new_reaction')]
+        obj['user'] = User._dese(res.get('user'))
+        obj['actor_chat'] = Chat._dese(res.get('actor_chat'))
         return cls(**obj)
 
     def __init__(
         self,
-        message_id: int
+        chat: Chat,
+        message_id: int,
+        date: int,
+        old_reaction: list[ReactionType],
+        new_reaction: list[ReactionType],
+        user: Optional[User] = None,
+        actor_chat: Optional[Chat] = None
     ):
+        self.chat = chat
         self.message_id = message_id
+        self.date = date
+        self.old_reaction = old_reaction
+        self.new_reaction = new_reaction
+        self.user = user
+        self.actor_chat = actor_chat
 
 
-class PhotoSize(TelegramType):
+class OrderInfo(TelegramType):
     '''
-    https://core.telegram.org/bots/api#photosize
+    https://core.telegram.org/bots/api#orderinfo
+
+    This object represents information about an order.
 
-    This object represents one size of a photo or a file / sticker thumbnail.
+    :param name: User name.
+    :type name: :obj:`str`, optional
+    :param phone_number: User's phone number.
+    :type phone_number: :obj:`str`, optional
+    :param email: User email.
+    :type email: :obj:`str`, optional
+    :param shipping_address: User shipping address.
+    :type shipping_address: :obj:`~aiotgm.types.ShippingAddress`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['file_id'] = res.get('file_id')
-        obj['file_unique_id'] = res.get('file_unique_id')
-        obj['width'] = res.get('width')
-        obj['height'] = res.get('height')
-        obj['file_size'] = res.get('file_size')
+        obj['name'] = res.get('name')
+        obj['phone_number'] = res.get('phone_number')
+        obj['email'] = res.get('email')
+        obj['shipping_address'] = ShippingAddress._dese(res.get('shipping_address'))
         return cls(**obj)
 
     def __init__(
         self,
-        file_id: str,
-        file_unique_id: str,
-        width: int,
-        height: int,
-        file_size: Optional[int] = None
+        name: Optional[str] = None,
+        phone_number: Optional[str] = None,
+        email: Optional[str] = None,
+        shipping_address: Optional[ShippingAddress] = None
     ):
-        self.file_id = file_id
-        self.file_unique_id = file_unique_id
-        self.width = width
-        self.height = height
-        self.file_size = file_size
+        self.name = name
+        self.phone_number = phone_number
+        self.email = email
+        self.shipping_address = shipping_address
 
 
-class Story(TelegramType):
+class PassportData(TelegramType):
     '''
-    https://core.telegram.org/bots/api#story
+    https://core.telegram.org/bots/api#passportdata
+
+    Describes Telegram Passport data shared with the bot by the user.
 
-    This object represents a message about a forwarded story in the chat. Currently holds no information.
+    :param data: Array with information about documents and other Telegram Passport elements that was shared with the bot.
+    :type data: :obj:`list` of :obj:`~aiotgm.types.EncryptedPassportElement`
+    :param credentials: Encrypted credentials required to decrypt the data.
+    :type credentials: :obj:`~aiotgm.types.EncryptedCredentials`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['chat'] = Chat._dese(res.get('chat'))
-        obj['id'] = res.get('id')
+        obj['data'] = [EncryptedPassportElement._dese(kwargs) for kwargs in res.get('data')]
+        obj['credentials'] = EncryptedCredentials._dese(res.get('credentials'))
         return cls(**obj)
 
     def __init__(
         self,
-        chat: Chat,
-        id: int
+        data: list[EncryptedPassportElement],
+        credentials: EncryptedCredentials
     ):
-        self.chat = chat
-        self.id = id
+        self.data = data
+        self.credentials = credentials
 
 
-class Video(TelegramType):
+class PassportElementErrorDataField(TelegramType):
     '''
-    https://core.telegram.org/bots/api#video
+    https://core.telegram.org/bots/api#passportelementerrordatafield
 
-    This object represents a video file.
+    Represents an issue in one of the data fields that was provided by the user.
+    The error is considered resolved when the field's value changes.
+
+    :param type: The section of the user's Telegram Passport which has the error, one of “personal_details”, “passport”, “driver_license”, “identity_card”, “internal_passport”, “address”.
+    :type type: :obj:`str`
+    :param field_name: Name of the data field which has the error.
+    :type field_name: :obj:`str`
+    :param data_hash: Base64-encoded data hash.
+    :type data_hash: :obj:`str`
+    :param message: Error message.
+    :type message: :obj:`str`
     '''
-    @classmethod
-    @_parse_result
-    def _dese(cls, res: dict):
-        obj = {}
-        obj['file_id'] = res.get('file_id')
-        obj['file_unique_id'] = res.get('file_unique_id')
-        obj['width'] = res.get('width')
-        obj['height'] = res.get('height')
-        obj['duration'] = res.get('duration')
-        obj['thumbnail'] = PhotoSize._dese(res.get('thumbnail'))
-        obj['file_name'] = res.get('file_name')
-        obj['mime_type'] = res.get('mime_type')
-        obj['file_size'] = res.get('file_size')
-        return cls(**obj)
+    def __init__(
+        self,
+        type: str,
+        field_name: str,
+        data_hash: str,
+        message: str
+    ):
+        self.source = DEFAULT_PASSPORT_ELEMENT_ERROR_DATA_FIELD
+        self.type = type
+        self.field_name = field_name
+        self.data_hash = data_hash
+        self.message = message
 
+
+class PassportElementErrorFile(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#passportelementerrorfile
+
+    Represents an issue with a document scan.
+    The error is considered resolved when the file with the document scan changes.
+
+    :param type: The section of the user's Telegram Passport which has the issue, one of “utility_bill”, “bank_statement”, “rental_agreement”, “passport_registration”, “temporary_registration”.
+    :type type: :obj:`str`
+    :param file_hash: Base64-encoded file hash.
+    :type file_hash: :obj:`str`
+    :param message: Error message.
+    :type message: :obj:`str`
+    '''
     def __init__(
         self,
-        file_id: str,
-        file_unique_id: str,
-        width: int,
-        height: int,
-        duration: int,
-        thumbnail: Optional[PhotoSize] = None,
-        file_name: Optional[str] = None,
-        mime_type: Optional[str] = None,
-        file_size: Optional[int] = None
+        type: str,
+        file_hash: str,
+        message: str
     ):
-        self.file_id = file_id
-        self.file_unique_id = file_unique_id
-        self.width = width
-        self.height = height
-        self.duration = duration
-        self.thumbnail = thumbnail
-        self.file_name = file_name
-        self.mime_type = mime_type
-        self.file_size = file_size
+        self.source = DEFAULT_PASSPORT_ELEMENT_ERROR_FILE
+        self.type = type
+        self.file_hash = file_hash
+        self.message = message
 
 
-class VideoNote(TelegramType):
+class PassportElementErrorFiles(TelegramType):
     '''
-    https://core.telegram.org/bots/api#videonote
+    https://core.telegram.org/bots/api#passportelementerrorfiles
 
-    This object represents a video message (available in Telegram apps as of v.4.0).
+    Represents an issue with a list of scans.
+    The error is considered resolved when the list of files containing the scans changes.
+
+    :param type: The section of the user's Telegram Passport which has the issue, one of “utility_bill”, “bank_statement”, “rental_agreement”, “passport_registration”, “temporary_registration”.
+    :type type: :obj:`str`
+    :param file_hashes: List of base64-encoded file hashes.
+    :type file_hashes: :obj:`list` of :obj:`str`
+    :param message: Error message.
+    :type message: :obj:`str`
     '''
-    @classmethod
-    @_parse_result
-    def _dese(cls, res: dict):
-        obj = {}
-        obj['file_id'] = res.get('file_id')
-        obj['file_unique_id'] = res.get('file_unique_id')
-        obj['length'] = res.get('length')
-        obj['duration'] = res.get('duration')
-        obj['thumbnail'] = PhotoSize._dese(res.get('thumbnail'))
-        obj['file_size'] = res.get('file_size')
-        return cls(**obj)
+    def __init__(
+        self,
+        type: str,
+        file_hashes: list[str],
+        message: str
+    ):
+        self.source = DEFAULT_PASSPORT_ELEMENT_ERROR_FILES
+        self.type = type
+        self.file_hashes = file_hashes
+        self.message = message
 
+
+class PassportElementErrorFrontSide(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#passportelementerrorfrontside
+
+    Represents an issue with the front side of a document.
+    The error is considered resolved when the file with the front side of the document changes.
+
+    :param type: The section of the user's Telegram Passport which has the issue, one of “passport”, “driver_license”, “identity_card”, “internal_passport”.
+    :type type: :obj:`str`
+    :param file_hash: Base64-encoded hash of the file with the front side of the document.
+    :type file_hash: :obj:`str`
+    :param message: Error message.
+    :type message: :obj:`str`
+    '''
     def __init__(
         self,
-        file_id: str,
-        file_unique_id: str,
-        length: int,
-        duration: int,
-        thumbnail: Optional[PhotoSize] = None,
-        file_size: Optional[int] = None
+        type: str,
+        file_hash: str,
+        message: str
     ):
-        self.file_id = file_id
-        self.file_unique_id = file_unique_id
-        self.length = length
-        self.duration = duration
-        self.thumbnail = thumbnail
-        self.file_size = file_size
+        self.source = DEFAULT_PASSPORT_ELEMENT_ERROR_FRONT_SIDE
+        self.type = type
+        self.file_hash = file_hash
+        self.message = message
 
 
-class Voice(TelegramType):
+class PassportElementErrorReverseSide(TelegramType):
     '''
-    https://core.telegram.org/bots/api#voice
+    https://core.telegram.org/bots/api#passportelementerrorreverseside
 
-    This object represents a voice note.
+    Represents an issue with the reverse side of a document.
+    The error is considered resolved when the file with reverse side of the document changes.
+
+    :param type: The section of the user's Telegram Passport which has the issue, one of “driver_license”, “identity_card”.
+    :type type: :obj:`str`
+    :param file_hash: Base64-encoded hash of the file with the reverse side of the document.
+    :type file_hash: :obj:`str`
+    :param message: Error message.
+    :type message: :obj:`str`
     '''
-    @classmethod
-    @_parse_result
-    def _dese(cls, res: dict):
-        obj = {}
-        obj['file_id'] = res.get('file_id')
-        obj['file_unique_id'] = res.get('file_unique_id')
-        obj['duration'] = res.get('duration')
-        obj['mime_type'] = res.get('mime_type')
-        obj['file_size'] = res.get('file_size')
-        return cls(**obj)
+    def __init__(
+        self,
+        type: str,
+        file_hash: str,
+        message: str
+    ):
+        self.source = DEFAULT_PASSPORT_ELEMENT_ERROR_REVERSE_SIDE
+        self.type = type
+        self.file_hash = file_hash
+        self.message = message
+
+
+class PassportElementErrorSelfie(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#passportelementerrorselfie
 
+    Represents an issue with the selfie with a document.
+    The error is considered resolved when the file with the selfie changes.
+
+    :param type: The section of the user's Telegram Passport which has the issue, one of “passport”, “driver_license”, “identity_card”, “internal_passport”.
+    :type type: :obj:`str`
+    :param file_hash: Base64-encoded hash of the file with the selfie.
+    :type file_hash: :obj:`str`
+    :param message: Error message.
+    :type message: :obj:`str`
+    '''
     def __init__(
         self,
-        file_id: str,
-        file_unique_id: str,
-        duration: int,
-        mime_type: Optional[str] = None,
-        file_size: Optional[int] = None
+        type: str,
+        file_hash: str,
+        message: str
     ):
-        self.file_id = file_id
-        self.file_unique_id = file_unique_id
-        self.duration = duration
-        self.mime_type = mime_type
-        self.file_size = file_size
+        self.source = DEFAULT_PASSPORT_ELEMENT_ERROR_SELFIE
+        self.type = type
+        self.file_hash = file_hash
+        self.message = message
 
 
-class PollOption(TelegramType):
+class PassportElementErrorTranslationFile(TelegramType):
     '''
-    https://core.telegram.org/bots/api#polloption
+    https://core.telegram.org/bots/api#passportelementerrortranslationfile
 
-    This object contains information about one answer option in a poll.
+    Represents an issue with one of the files that constitute the translation of a document.
+    The error is considered resolved when the file changes.
+
+    :param type: Type of element of the user's Telegram Passport which has the issue, one of “passport”, “driver_license”, “identity_card”, “internal_passport”, “utility_bill”, “bank_statement”, “rental_agreement”, “passport_registration”, “temporary_registration”.
+    :type type: :obj:`str`
+    :param file_hash: Base64-encoded file hash.
+    :type file_hash: :obj:`str`
+    :param message: Error message.
+    :type message: :obj:`str`
+    '''
+    def __init__(
+        self,
+        type: str,
+        file_hash: str,
+        message: str
+    ):
+        self.source = DEFAULT_PASSPORT_ELEMENT_ERROR_TRANSLATION_FILE
+        self.type = type
+        self.file_hash = file_hash
+        self.message = message
+
+
+class PassportElementErrorTranslationFiles(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#passportelementerrortranslationfiles
+
+    Represents an issue with the translated version of a document.
+    The error is considered resolved when a file with the document translation change.
+
+    :param type: Type of element of the user's Telegram Passport which has the issue, one of “passport”, “driver_license”, “identity_card”, “internal_passport”, “utility_bill”, “bank_statement”, “rental_agreement”, “passport_registration”, “temporary_registration”.
+    :type type: :obj:`str`
+    :param file_hashes: List of base64-encoded file hashes.
+    :type file_hashes: :obj:`list` of :obj:`str`
+    :param message: Error message.
+    :type message: :obj:`str`
+    '''
+    def __init__(
+        self,
+        type: str,
+        file_hashes: list[str],
+        message: str
+    ):
+        self.source = DEFAULT_PASSPORT_ELEMENT_ERROR_TRANSLATION_FILES
+        self.type = type
+        self.file_hashes = file_hashes
+        self.message = message
+
+
+class PassportElementErrorUnspecified(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#passportelementerrorunspecified
+
+    Represents an issue in an unspecified place.
+    The error is considered resolved when new data is added.
+
+    :param type: Type of element of the user's Telegram Passport which has the issue.
+    :type type: :obj:`str`
+    :param element_hash: Base64-encoded element hash.
+    :type element_hash: :obj:`str`
+    :param message: Error message.
+    :type message: :obj:`str`
+    '''
+    def __init__(
+        self,
+        type: str,
+        element_hash: str,
+        message: str
+    ):
+        self.source = DEFAULT_PASSPORT_ELEMENT_ERROR_UNSPECIFIED
+        self.type = type
+        self.element_hash = element_hash
+        self.message = message
+
+
+class PassportFile(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#passportfile
+
+    This object represents a file uploaded to Telegram Passport.
+    Currently all Telegram Passport files are in JPEG format when decrypted and don't exceed 10MB.
+
+    :param file_id: Identifier for this file, which can be used to download or reuse the file.
+    :type file_id: :obj:`str`
+    :param file_unique_id: Unique identifier for this file, which is supposed to be the same over time and for different bots. Can't be used to download or reuse the file.
+    :type file_unique_id: :obj:`str`
+    :param file_size: File size in bytes.
+    :type file_size: :obj:`int`
+    :param file_date: Unix time when the file was uploaded.
+    :type file_date: :obj:`int`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['text'] = res.get('text')
-        obj['voter_count'] = res.get('voter_count')
+        obj['file_id'] = res.get('file_id')
+        obj['file_unique_id'] = res.get('file_unique_id')
+        obj['file_size'] = res.get('file_size')
+        obj['file_date'] = res.get('file_date')
         return cls(**obj)
 
     def __init__(
         self,
-        text: str,
-        voter_count: int
+        file_id: str,
+        file_unique_id: str,
+        file_size: int,
+        file_date: int
     ):
-        self.text = text
-        self.voter_count = voter_count
+        self.file_id = file_id
+        self.file_unique_id = file_unique_id
+        self.file_size = file_size
+        self.file_date = file_date
 
 
-class PollAnswer(TelegramType):
+class PhotoSize(TelegramType):
     '''
-    https://core.telegram.org/bots/api#pollanswer
+    https://core.telegram.org/bots/api#photosize
 
-    This object represents an answer of a user in a non-anonymous poll.
+    This object represents one size of a photo or a
+    :obj:`file <aiotgm.types.Document>` / :obj:`sticker <aiotgm.types.Sticker>` thumbnail.
+
+    :param file_id: Identifier for this file, which can be used to download or reuse the file.
+    :type file_id: :obj:`str`
+    :param file_unique_id: Unique identifier for this file, which is supposed to be the same over time and for different bots. Can't be used to download or reuse the file.
+    :type file_unique_id: :obj:`str`
+    :param width: Photo width.
+    :type width: :obj:`int`
+    :param height: Photo height.
+    :type height: :obj:`int`
+    :param file_size: File size in bytes.
+    :type file_size: :obj:`int`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['poll_id'] = res.get('poll_id')
-        obj['option_ids'] = res.get('option_ids')
-        obj['voter_chat'] = Chat._dese(res.get('voter_chat'))
-        obj['user'] = User._dese(res.get('user'))
+        obj['file_id'] = res.get('file_id')
+        obj['file_unique_id'] = res.get('file_unique_id')
+        obj['width'] = res.get('width')
+        obj['height'] = res.get('height')
+        obj['file_size'] = res.get('file_size')
         return cls(**obj)
 
     def __init__(
         self,
-        poll_id: str,
-        option_ids: list[int],
-        voter_chat: Optional[Chat] = None,
-        user: Optional[User] = None
+        file_id: str,
+        file_unique_id: str,
+        width: int,
+        height: int,
+        file_size: Optional[int] = None
     ):
-        self.poll_id = poll_id
-        self.option_ids = option_ids
-        self.voter_chat = voter_chat
-        self.user = user
+        self.file_id = file_id
+        self.file_unique_id = file_unique_id
+        self.width = width
+        self.height = height
+        self.file_size = file_size
 
 
 class Poll(TelegramType):
     '''
     https://core.telegram.org/bots/api#poll
 
     This object contains information about a poll.
+
+    :param id: Unique poll identifier.
+    :type id: :obj:`str`
+    :param question: Poll question, 1-300 characters.
+    :type question: :obj:`str`
+    :param options: List of poll options.
+    :type options: :obj:`list` of :obj:`~aiotgm.types.PollOption`
+    :param total_voter_count: Total number of users that voted in the poll.
+    :type total_voter_count: :obj:`int`
+    :param is_closed: :obj:`True`, if the poll is closed.
+    :type is_closed: :obj:`bool`
+    :param is_anonymous: :obj:`True`, if the poll is anonymous.
+    :type is_anonymous: :obj:`bool`
+    :param type: Poll type, currently can be “regular” or “quiz”.
+    :type type: :obj:`str`
+    :param allows_multiple_answers: :obj:`True`, if the poll allows multiple answers.
+    :type allows_multiple_answers: :obj:`bool`
+    :param correct_option_id: 0-based identifier of the correct answer option. Available only for polls in the quiz mode, which are closed, or was sent (not forwarded) by the bot or to the private chat with the bot.
+    :type correct_option_id: :obj:`int`, optional
+    :param explanation: Text that is shown when a user chooses an incorrect answer or taps on the lamp icon in a quiz-style poll, 0-200 characters.
+    :type explanation: :obj:`str`, optional
+    :param explanation_entities: Special entities like usernames, URLs, bot commands, etc. that appear in the *explanation*.
+    :type explanation_entities: :obj:`list` of :obj:`~aiotgm.types.MessageEntity`, optional
+    :param open_period: Amount of time in seconds the poll will be active after creation.
+    :type open_period: :obj:`int`, optional
+    :param close_date: Point in time (Unix timestamp) when the poll will be automatically closed.
+    :type close_date: :obj:`int`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
         obj['id'] = res.get('id')
         obj['question'] = res.get('question')
@@ -5797,434 +6531,265 @@
         self.correct_option_id = correct_option_id
         self.explanation = explanation
         self.explanation_entities = explanation_entities
         self.open_period = open_period
         self.close_date = close_date
 
 
-class Venue(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#venue
-
-    This object represents a venue.
+class PollAnswer(TelegramType):
     '''
-    @classmethod
-    @_parse_result
-    def _dese(cls, res: dict):
-        obj = {}
-        obj['location'] = Location._dese(res.get('location'))
-        obj['title'] = res.get('title')
-        obj['address'] = res.get('address')
-        obj['foursquare_id'] = res.get('foursquare_id')
-        obj['foursquare_type'] = res.get('foursquare_type')
-        obj['google_place_id'] = res.get('google_place_id')
-        obj['google_place_type'] = res.get('google_place_type')
-        return cls(**obj)
-
-    def __init__(
-        self,
-        location: Location,
-        title: str,
-        address: str,
-        foursquare_id: Optional[str] = None,
-        foursquare_type: Optional[str] = None,
-        google_place_id: Optional[str] = None,
-        google_place_type: Optional[str] = None
-    ):
-        self.location = location
-        self.title = title
-        self.address = address
-        self.foursquare_id = foursquare_id
-        self.foursquare_type = foursquare_type
-        self.google_place_id = google_place_id
-        self.google_place_type = google_place_type
-
+    https://core.telegram.org/bots/api#pollanswer
 
-class WebAppData(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#webappdata
+    This object represents an answer of a user in a non-anonymous poll.
 
-    Describes data sent from a Web App to the bot.
+    :param poll_id: Unique poll identifier.
+    :type poll_id: :obj:`str`
+    :param option_ids: 0-based identifiers of chosen answer options. May be empty if the vote was retracted.
+    :type option_ids: :obj:`list` of :obj:`int`
+    :param voter_chat: The chat that changed the answer to the poll, if the voter is anonymous.
+    :type voter_chat: :obj:`~aiotgm.types.Chat`, optional
+    :param user: The user that changed the answer to the poll, if the voter isn't anonymous.
+    :type user: :obj:`~aiotgm.types.User`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['data'] = res.get('data')
-        obj['button_text'] = res.get('button_text')
+        obj['poll_id'] = res.get('poll_id')
+        obj['option_ids'] = res.get('option_ids')
+        obj['voter_chat'] = Chat._dese(res.get('voter_chat'))
+        obj['user'] = User._dese(res.get('user'))
         return cls(**obj)
 
     def __init__(
         self,
-        data: str,
-        button_text: str
+        poll_id: str,
+        option_ids: list[int],
+        voter_chat: Optional[Chat] = None,
+        user: Optional[User] = None
     ):
-        self.data = data
-        self.button_text = button_text
-
+        self.poll_id = poll_id
+        self.option_ids = option_ids
+        self.voter_chat = voter_chat
+        self.user = user
 
-class ProximityAlertTriggered(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#proximityalerttriggered
 
-    This object represents the content of a service message, sent whenever
-    a user in the chat triggers a proximity alert set by another user.
+class PollOption(TelegramType):
     '''
-    @classmethod
-    @_parse_result
-    def _dese(cls, res: dict):
-        obj = {}
-        obj['traveler'] = User._dese(res.get('traveler'))
-        obj['watcher'] = User._dese(res.get('watcher'))
-        obj['distance'] = res.get('distance')
-        return cls(**obj)
-
-    def __init__(
-        self,
-        traveler: User,
-        watcher: User,
-        distance: int
-    ):
-        self.traveler = traveler
-        self.watcher = watcher
-        self.distance = distance
-
+    https://core.telegram.org/bots/api#polloption
 
-class MessageAutoDeleteTimerChanged(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#messageautodeletetimerchanged
+    This object contains information about one answer option in a poll.
 
-    This object represents a service message about a change in auto-delete timer settings.
+    :param text: Option text, 1-100 characters.
+    :type text: :obj:`str`
+    :param voter_count: Number of users that voted for this option.
+    :type voter_count: :obj:`int`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['message_auto_delete_time'] = res.get('message_auto_delete_time')
+        obj['text'] = res.get('text')
+        obj['voter_count'] = res.get('voter_count')
         return cls(**obj)
 
     def __init__(
         self,
-        message_auto_delete_time: int
+        text: str,
+        voter_count: int
     ):
-        self.message_auto_delete_time = message_auto_delete_time
-
+        self.text = text
+        self.voter_count = voter_count
 
-class UsersShared(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#usersshared
 
-    This object contains information about the users whose identifiers
-    were shared with the bot using a KeyboardButtonRequestUsers button.
+class PreCheckoutQuery(TelegramType):
     '''
-    @classmethod
-    @_parse_result
-    def _dese(cls, res: dict):
-        obj = {}
-        obj['request_id'] = res.get('request_id')
-        obj['users'] = [SharedUser._dese(kwargs) for kwargs in res.get('users')]
-        return cls(**obj)
-
-    def __init__(
-        self,
-        request_id: int,
-        users: list[SharedUser]
-    ):
-        self.request_id = request_id
-        self.users = users
-
+    https://core.telegram.org/bots/api#precheckoutquery
 
-class WriteAccessAllowed(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#writeaccessallowed
+    This object contains information about an incoming pre-checkout query.
 
-    This object represents a service message about a user allowing a bot to write
-    messages after adding it to the attachment menu, launching a Web App from a link,
-    or accepting an explicit request from a Web App sent by the method requestWriteAccess.
+    :param id: Unique query identifier.
+    :type id: :obj:`str`
+    :param from_user: User who sent the query.
+    :type from_user: :obj:`~aiotgm.types.User`
+    :param currency: Three-letter ISO 4217 `currency <https://core.telegram.org/bots/payments#supported-currencies>`_ code.
+    :type currency: :obj:`str`
+    :param total_amount: Total price in the *smallest units* of the currency (integer, **not** float/double). For example, for a price of ``US$ 1.45`` pass ``amount = 145``. See the *exp* parameter in `currencies.json <https://core.telegram.org/bots/payments/currencies.json>`_, it shows the number of digits past the decimal point for each currency (2 for the majority of currencies).
+    :type total_amount: :obj:`int`
+    :param invoice_payload: Bot specified invoice payload.
+    :type invoice_payload: :obj:`str`
+    :param shipping_option_id: Identifier of the shipping option chosen by the user.
+    :type shipping_option_id: :obj:`str`, optional
+    :param order_info: Order information provided by the user.
+    :type order_info: :obj:`~aiotgm.types.OrderInfo`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['from_request'] = res.get('from_request')
-        obj['web_app_name'] = res.get('web_app_name')
-        obj['from_attachment_menu'] = res.get('from_attachment_menu')
+        obj['id'] = res.get('id')
+        obj['from_user'] = User._dese(res.get('from_user'))
+        obj['currency'] = res.get('currency')
+        obj['total_amount'] = res.get('total_amount')
+        obj['invoice_payload'] = res.get('invoice_payload')
+        obj['shipping_option_id'] = res.get('shipping_option_id')
+        obj['order_info'] = OrderInfo._dese(res.get('order_info'))
         return cls(**obj)
 
     def __init__(
         self,
-        from_request: Optional[bool] = None,
-        web_app_name: Optional[str] = None,
-        from_attachment_menu: Optional[bool] = None
+        id: str,
+        from_user: User,
+        currency: str,
+        total_amount: int,
+        invoice_payload: str,
+        shipping_option_id: Optional[str] = None,
+        order_info: Optional[OrderInfo] = None
     ):
-        self.from_request = from_request
-        self.web_app_name = web_app_name
-        self.from_attachment_menu = from_attachment_menu
+        self.id = id
+        self.from_user = from_user
+        self.currency = currency
+        self.total_amount = total_amount
+        self.invoice_payload = invoice_payload
+        self.shipping_option_id = shipping_option_id
+        self.order_info = order_info
 
 
-class VideoChatScheduled(TelegramType):
+class ProximityAlertTriggered(TelegramType):
     '''
-    https://core.telegram.org/bots/api#videochatscheduled
+    https://core.telegram.org/bots/api#proximityalerttriggered
 
-    This object represents a service message about a video chat scheduled in the chat.
+    This object represents the content of a service message, sent whenever
+    a user in the chat triggers a proximity alert set by another user.
+
+    :param traveler: User that triggered the alert.
+    :type traveler: :obj:`~aiotgm.types.User`
+    :param watcher: User that set the alert.
+    :type watcher: :obj:`~aiotgm.types.User`
+    :param distance: The distance between the users.
+    :type distance: :obj:`int`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['start_date'] = res.get('start_date')
+        obj['traveler'] = User._dese(res.get('traveler'))
+        obj['watcher'] = User._dese(res.get('watcher'))
+        obj['distance'] = res.get('distance')
         return cls(**obj)
 
     def __init__(
         self,
-        start_date: int
+        traveler: User,
+        watcher: User,
+        distance: int
     ):
-        self.start_date = start_date
-
+        self.traveler = traveler
+        self.watcher = watcher
+        self.distance = distance
 
-class VideoChatStarted(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#videochatstarted
 
-    This object represents a service message about a video
-    chat started in the chat. Currently holds no information.
+class ReactionCount(TelegramType):
     '''
-    @classmethod
-    @_parse_result
-    def _dese(cls, res: dict):
-        obj = {}
-        return cls(**obj)
-
-    def __init__(self):
-        ...
-
+    https://core.telegram.org/bots/api#reactioncount
 
-class VideoChatEnded(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#videochatended
+    Represents a reaction added to a message along with the number of times it was added.
 
-    This object represents a service message about a video chat ended in the chat.
+    :param type: Type of the reaction.
+    :type type: :obj:`~aiotgm.types.ReactionType`
+    :param total_count: Number of times the reaction was added.
+    :type total_count: :obj:`int`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['duration'] = res.get('duration')
+        obj['type'] = _dese_reaction_type(res.get('type'))
+        obj['total_count'] = res.get('total_count')
         return cls(**obj)
 
     def __init__(
         self,
-        duration: int
+        type: ReactionType,
+        total_count: int
     ):
-        self.duration = duration
-
+        self.type = type
+        self.total_count = total_count
 
-class VideoChatParticipantsInvited(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#videochatparticipantsinvited
 
-    This object represents a service message about new members invited to a video chat.
+class ReactionTypeCustomEmoji(TelegramType):
     '''
-    @classmethod
-    @_parse_result
-    def _dese(cls, res: dict):
-        obj = {}
-        obj['users'] = [User._dese(kwargs) for kwargs in res.get('users')]
-        return cls(**obj)
-
-    def __init__(
-        self,
-        users: list[User]
-    ):
-        self.users = users
-
+    https://core.telegram.org/bots/api#reactiontypecustomemoji
 
-class SharedUser(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#shareduser
+    The reaction is based on a custom emoji.
 
-    This object contains information about a user that was shared with
-    the bot using a :obj:`~aiotgm.types.KeyboardButtonRequestUser` button.
+    :param custom_emoji_id: Custom emoji identifier.
+    :type custom_emoji_id: :obj:`str`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['user_id'] = res.get('user_id')
-        obj['first_name'] = res.get('first_name')
-        obj['last_name'] = res.get('last_name')
-        obj['username'] = res.get('username')
-        obj['photo'] = [PhotoSize._dese(kwargs) for kwargs in res.get('photo')] if 'photo' in res else None
+        obj['custom_emoji_id'] = res.get('custom_emoji_id')
         return cls(**obj)
 
     def __init__(
         self,
-        user_id: int,
-        first_name: Optional[str] = None,
-        last_name: Optional[str] = None,
-        username: Optional[str] = None,
-        photo: Optional[list[PhotoSize]] = None
+        custom_emoji_id: str
     ):
-        self.user_id = user_id
-        self.first_name = first_name
-        self.last_name = last_name
-        self.username = username
-        self.photo = photo
-
+        self.type = DEFAULT_REACTION_TYPE_CUSTOM_EMOJI
+        self.custom_emoji_id = custom_emoji_id
 
-class UserProfilePhotos(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#userprofilephotos
 
-    This object represent a user's profile pictures.
+class ReactionTypeEmoji(TelegramType):
     '''
-    @classmethod
-    @_parse_result
-    def _dese(cls, res: dict):
-        obj = {}
-        obj['total_count'] = res.get('total_count')
-        obj['photos'] = [[PhotoSize._dese(kwargs) for kwargs in lst] for lst in res.get('photos')]
-        return cls(**obj)
-
-    def __init__(
-        self,
-        total_count: int,
-        photos: list[list[PhotoSize]]
-    ):
-        self.total_count = total_count
-        self.photos = photos
-
+    https://core.telegram.org/bots/api#reactiontypeemoji
 
-class WebAppInfo(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#webappinfo
+    The reaction is based on an emoji.
 
-    Describes a Web App.
+    :param emoji: Reaction emoji. Currently, it can be one of "👍", "👎", "❤", "🔥", "🥰", "👏", "😁", "🤔", "🤯", "😱", "🤬", "😢", "🎉", "🤩", "🤮", "💩", "🙏", "👌", "🕊", "🤡", "🥱", "🥴", "😍", "🐳", "❤‍🔥", "🌚", "🌭", "💯", "🤣", "⚡", "🍌", "🏆", "💔", "🤨", "😐", "🍓", "🍾", "💋", "🖕", "😈", "😴", "😭", "🤓", "👻", "👨‍💻", "👀", "🎃", "🙈", "😇", "😨", "🤝", "✍", "🤗", "🫡", "🎅", "🎄", "☃", "💅", "🤪", "🗿", "🆒", "💘", "🙉", "🦄", "😘", "💊", "🙊", "😎", "👾", "🤷‍♂", "🤷", "🤷‍♀", "😡".
+    :type emoji: :obj:`str`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['url'] = res.get('url')
+        obj['emoji'] = res.get('emoji')
         return cls(**obj)
 
     def __init__(
         self,
-        url: str
-    ):
-        self.url = url
-
-
-class KeyboardButtonRequestUsers(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#keyboardbuttonrequestusers
-
-    This object defines the criteria used to request suitable users.\n
-    The identifiers of the selected users will be shared with the bot when the corresponding button is pressed.
-    '''
-    def __init__(
-        self,
-        request_id: int,
-        user_is_bot: Optional[bool] = None,
-        user_is_premium: Optional[bool] = None,
-        max_quantity: Optional[int] = None,
-        request_name: Optional[bool] = None,
-        request_username: Optional[bool] = None,
-        request_photo: Optional[bool] = None
-    ):
-        self.request_id = request_id
-        self.user_is_bot = user_is_bot
-        self.user_is_premium = user_is_premium
-        self.max_quantity = max_quantity
-        self.request_name = request_name
-        self.request_username = request_username
-        self.request_photo = request_photo
-
-
-class KeyboardButtonRequestChat(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#keyboardbuttonrequestchat
-
-    This object defines the criteria used to request a suitable chat.
-    The identifier of the selected chat will be shared with the bot when the corresponding button is pressed.
-    '''
-    def __init__(
-        self,
-        request_id: int,
-        chat_is_channel: bool,
-        chat_is_forum: Optional[bool] = None,
-        chat_has_username: Optional[bool] = None,
-        chat_is_created: Optional[bool] = None,
-        user_administrator_rights: Optional[ChatAdministratorRights] = None,
-        bot_administrator_rights: Optional[ChatAdministratorRights] = None,
-        bot_is_member: Optional[bool] = None,
-        request_title: Optional[bool] = None,
-        request_username: Optional[bool] = None,
-        request_photo: Optional[bool] = None
-    ):
-        self.request_id = request_id
-        self.chat_is_channel = chat_is_channel
-        self.chat_is_forum = chat_is_forum
-        self.chat_has_username = chat_has_username
-        self.chat_is_created = chat_is_created
-        self.user_administrator_rights = user_administrator_rights
-        self.bot_administrator_rights = bot_administrator_rights
-        self.bot_is_member = bot_is_member
-        self.request_title = request_title
-        self.request_username = request_username
-        self.request_photo = request_photo
-
-
-class KeyboardButtonPollType(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#keyboardbuttonpolltype
-
-    This object represents type of a poll, which is allowed to
-    be created and sent when the corresponding button is pressed.
-    '''
-    def __init__(
-        self,
-        type: Optional[str] = None
-    ):
-        self.type = type
-
-
-class KeyboardButton(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#keyboardbutton
-
-    This object represents one button of the reply keyboard.\n
-    For simple text buttons, String can be used instead of this object to specify the button text.\n
-    The optional fields web_app, request_users, request_chat, request_contact, request_location, and request_poll are mutually exclusive.
-    '''
-    def __init__(
-        self,
-        text: str,
-        request_users: Optional[KeyboardButtonRequestUsers] = None,
-        request_chat: Optional[KeyboardButtonRequestChat] = None,
-        request_contact: Optional[bool] = None,
-        request_location: Optional[bool] = None,
-        request_poll: Optional[KeyboardButtonPollType] = None,
-        web_app: Optional[WebAppInfo] = None
+        emoji: str
     ):
-        self.text = text
-        self.request_users = request_users
-        self.request_chat = request_chat
-        self.request_contact = request_contact
-        self.request_location = request_location
-        self.request_poll = request_poll
-        self.web_app = web_app
+        self.type = DEFAULT_REACTION_TYPE_EMOJI
+        self.emoji = emoji
 
 
 class ReplyKeyboardMarkup(TelegramType):
     '''
     https://core.telegram.org/bots/api#replykeyboardmarkup
 
-    This object represents a custom keyboard with reply
-    options (see Introduction to bots for details and examples).
+    This object represents a `custom keyboard <https://core.telegram.org/bots/features#keyboards>`_ with reply
+    options (see `Introduction to bots <https://core.telegram.org/bots/features#keyboards>`_ for details and examples).
+
+    :param keyboard: Array of button rows, each represented by an Array of :obj:`~aiotgm.types.KeyboardButton` objects.
+    :type keyboard: :obj:`list` of :obj:`list` of :obj:`~aiotgm.types.KeyboardButton`, optional
+    :param is_persistent: Requests clients to always show the keyboard when the regular keyboard is hidden. Defaults to :obj:`False`, in which case the custom keyboard can be hidden and opened with a keyboard icon.
+    :type is_persistent: :obj:`bool`, optional
+    :param resize_keyboard: Requests clients to resize the keyboard vertically for optimal fit (e.g., make the keyboard smaller if there are just two rows of buttons). Defaults to :obj:`False`, in which case the custom keyboard is always of the same height as the app's standard keyboard.
+    :type resize_keyboard: :obj:`bool`, optional
+    :param one_time_keyboard: Requests clients to hide the keyboard as soon as it's been used. The keyboard will still be available, but clients will automatically display the usual letter-keyboard in the chat - the user can press a special button in the input field to see the custom keyboard again. Defaults to :obj:`False`.
+    :type one_time_keyboard: :obj:`bool`, optional
+    :param input_field_placeholder: The placeholder to be shown in the input field when the keyboard is active; 1-64 characters.
+    :type input_field_placeholder: :obj:`str`, optional
+    :param selective:
+        Use this parameter if you want to show the keyboard to specific users only. Targets: 1) users that are @mentioned in the *text* of the :obj:`~aiotgm.types.Message` object; 2) if the bot's message is a reply to a message in the same chat and forum topic, sender of the original message.
+
+        *Example*: A user requests to change the bot's language, bot replies to the request with a keyboard to select the new language. Other users in the group don't see the keyboard.
+    :type selective: :obj:`bool`, optional
     '''
     def __init__(
         self,
         keyboard: Optional[list[list[KeyboardButton]]] = None,
         is_persistent: Optional[bool] = None,
         resize_keyboard: Optional[bool] = None,
         one_time_keyboard: Optional[bool] = None,
@@ -6295,192 +6860,314 @@
         self.keyboard = keyboard
 
 
 class ReplyKeyboardRemove(TelegramType):
     '''
     https://core.telegram.org/bots/api#replykeyboardremove
 
-    Upon receiving a message with this object, Telegram clients will remove the current custom keyboard and display the default letter-keyboard.\n
-    By default, custom keyboards are displayed until a new keyboard is sent by a bot.\n
-    An exception is made for one-time keyboards that are hidden immediately after the user presses a button (see ReplyKeyboardMarkup).
+    Upon receiving a message with this object, Telegram clients will remove the current custom keyboard
+    and display the default letter-keyboard. By default, custom keyboards are displayed until a new
+    keyboard is sent by a bot. An exception is made for one-time keyboards that are hidden immediately
+    after the user presses a button (see :obj:`~aiotgm.types.ReplyKeyboardMarkup`).
+
+    :param selective:
+        Use this parameter if you want to remove the keyboard for specific users only. Targets: 1) users that are @mentioned in the *text* of the :obj:`~aiotgm.types.Message` object; 2) if the bot's message is a reply to a message in the same chat and forum topic, sender of the original message.
+
+        *Example*: A user votes in a poll, bot returns confirmation message in reply to the vote and removes the keyboard for that user, while still showing the keyboard with poll options to users who haven't voted yet.
+    :type selective: :obj:`bool`, optional
     '''
     def __init__(
         self,
         selective: Optional[bool] = None
     ):
         self.remove_keyboard: Literal[True] = True
         self.selective = selective
 
 
-REPLY_MARKUP_TYPES = Union[InlineKeyboardMarkup, ReplyKeyboardMarkup, ReplyKeyboardRemove, ForceReply]
-'''
-One of the following reply markups:
+class ReplyParameters(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#replyparameters
 
-- :obj:`~aiotgm.types.InlineKeyboardMarkup`
-- :obj:`~aiotgm.types.ReplyKeyboardMarkup`
-- :obj:`~aiotgm.types.ReplyKeyboardRemove`
-- :obj:`~aiotgm.types.ForceReply`
-'''
+    Describes reply parameters for the message that is being sent.
+
+    :param message_id: Identifier of the message that will be replied to in the current chat, or in the chat chat_id if it is specified.
+    :type message_id: :obj:`int`
+    :param chat_id: If the message to be replied to is from a different chat, unique identifier for the chat or username of the channel (in the format ``@channelusername``). Not supported for messages sent on behalf of a business account.
+    :type chat_id: :obj:`int` or :obj:`str`, optional
+    :param allow_sending_without_reply: Pass :obj:`True` if the message should be sent even if the specified message to be replied to is not found. Always :obj:`False` for replies in another chat or forum topic. Always :obj:`True` for messages sent on behalf of a business account.
+    :type allow_sending_without_reply: :obj:`bool`, optional
+    :param quote: Quoted part of the message to be replied to; 0-1024 characters after entities parsing. The quote must be an exact substring of the message to be replied to, including *bold*, *italic*, *underline*, *strikethrough*, *spoiler*, and *custom_emoji entities*. The message will fail to send if the quote isn't found in the original message.
+    :type quote: :obj:`str`, optional
+    :param quote_parse_mode: Mode for parsing entities in the quote. See `formatting options <https://core.telegram.org/bots/api#formatting-options>`_ for more details.
+    :type quote_parse_mode: :obj:`str`, optional
+    :param quote_entities: A JSON-serialized list of special entities that appear in the quote. It can be specified instead of *quote_parse_mode*.
+    :type quote_entities: :obj:`list` of :obj:`~aiotgm.types.MessageEntity`, optional
+    :param quote_position: Position of the quote in the original message in UTF-16 code units.
+    :type quote_position: :obj:`int`, optional
+    '''
+    def __init__(
+        self,
+        message_id: int,
+        chat_id: Optional[Union[int, str]] = None,
+        allow_sending_without_reply: Optional[bool] = None,
+        quote: Optional[str] = None,
+        quote_parse_mode: Optional[str] = None,
+        quote_entities: Optional[list[MessageEntity]] = None,
+        quote_position: Optional[int] = None
+    ):
+        self.message_id = message_id
+        self.chat_id = chat_id
+        self.allow_sending_without_reply = allow_sending_without_reply
+        self.quote = quote
+        self.quote_parse_mode = quote_parse_mode
+        self.quote_entities = quote_entities
+        self.quote_position = quote_position
 
-# MenuButton: 3 SUBCLASSES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-class MenuButtonCommands(TelegramType):
+class ResponseParameters(TelegramType):
     '''
-    https://core.telegram.org/bots/api#menubuttoncommands
+    https://core.telegram.org/bots/api#responseparameters
 
-    Represents a menu button, which opens the bot's list of commands.
+    Describes why a request was unsuccessful.
+
+    :param migrate_to_chat_id: The group has been migrated to a supergroup with the specified identifier. This number may have more than 32 significant bits and some programming languages may have difficulty/silent defects in interpreting it. But it has at most 52 significant bits, so a signed 64-bit integer or double-precision float type are safe for storing this identifier.
+    :type migrate_to_chat_id: :obj:`int`, optional
+    :param retry_after: In case of exceeding flood control, the number of seconds left to wait before the request can be repeated.
+    :type retry_after: :obj:`int`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
+        obj['migrate_to_chat_id'] = res.get('migrate_to_chat_id')
+        obj['retry_after'] = res.get('retry_after')
         return cls(**obj)
 
-    def __init__(self):
-        self.type = DEFAULT_MENU_BUTTON_COMMANDS
+    def __init__(
+        self,
+        migrate_to_chat_id: Optional[int] = None,
+        retry_after: Optional[int] = None
+    ):
+        self.migrate_to_chat_id = migrate_to_chat_id
+        self.retry_after = retry_after
 
 
-class MenuButtonWebApp(TelegramType):
+class SentWebAppMessage(TelegramType):
     '''
-    https://core.telegram.org/bots/api#menubuttonwebapp
+    https://core.telegram.org/bots/api#sentwebappmessage
+
+    Describes an inline message sent by a `Web App <https://core.telegram.org/bots/webapps>`_ on behalf of a user.
 
-    Represents a menu button, which launches a Web App.
+    :param inline_message_id: Identifier of the sent inline message. Available only if there is an :obj:`inline keyboard <aiotgm.types.InlineKeyboardMarkup>` attached to the message.
+    :type inline_message_id: :obj:`str`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['text'] = res.get('text')
-        obj['web_app'] = WebAppInfo._dese(res.get('web_app'))
+        obj['inline_message_id'] = res.get('inline_message_id')
         return cls(**obj)
 
     def __init__(
         self,
-        text: str,
-        web_app: WebAppInfo
+        inline_message_id: Optional[str] = None
     ):
-        self.type = DEFAULT_MENU_BUTTON_WEB_APP
-        self.text = text
-        self.web_app = web_app
+        self.inline_message_id = inline_message_id
 
 
-class MenuButtonDefault(TelegramType):
+class SharedUser(TelegramType):
     '''
-    https://core.telegram.org/bots/api#menubuttondefault
+    https://core.telegram.org/bots/api#shareduser
 
-    Describes that no specific value for the menu button was set.
+    This object contains information about a user that was shared with
+    the bot using a :obj:`~aiotgm.types.KeyboardButtonRequestUsers` button.
+
+    :param user_id: Identifier of the shared user. This number may have more than 32 significant bits and some programming languages may have difficulty/silent defects in interpreting it. But it has at most 52 significant bits, so 64-bit integers or double-precision float types are safe for storing these identifiers. The bot may not have access to the user and could be unable to use this identifier, unless the user is already known to the bot by some other means.
+    :type user_id: :obj:`int`
+    :param first_name: First name of the user, if the name was requested by the bot.
+    :type first_name: :obj:`str`, optional
+    :param last_name: Last name of the user, if the name was requested by the bot.
+    :type last_name: :obj:`str`, optional
+    :param username: Username of the user, if the username was requested by the bot.
+    :type username: :obj:`str`, optional
+    :param photo: Available sizes of the chat photo, if the photo was requested by the bot.
+    :type photo: :obj:`list` of :obj:`~aiotgm.types.PhotoSize`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
+        obj['user_id'] = res.get('user_id')
+        obj['first_name'] = res.get('first_name')
+        obj['last_name'] = res.get('last_name')
+        obj['username'] = res.get('username')
+        obj['photo'] = [PhotoSize._dese(kwargs) for kwargs in res.get('photo')] if 'photo' in res else None
         return cls(**obj)
 
-    def __init__(self):
-        self.type = DEFAULT_MENU_BUTTON_DEFAULT
-
-
-MenuButton = Union[MenuButtonCommands, MenuButtonWebApp, MenuButtonDefault]
-'''
-https://core.telegram.org/bots/api#menubutton
-
-This object describes the bot's menu button in a private chat. It should be one of
-
-- MenuButtonCommands
-- MenuButtonWebApp
-- MenuButtonDefault
-
-If a menu button other than MenuButtonDefault is set for a private chat, then it is applied in the chat.
+    def __init__(
+        self,
+        user_id: int,
+        first_name: Optional[str] = None,
+        last_name: Optional[str] = None,
+        username: Optional[str] = None,
+        photo: Optional[list[PhotoSize]] = None
+    ):
+        self.user_id = user_id
+        self.first_name = first_name
+        self.last_name = last_name
+        self.username = username
+        self.photo = photo
 
-Otherwise the default menu button is applied. By default, the menu button opens the list of bot commands.
-'''
 
-def _dese_menu_button(res: Optional[dict], /) -> Optional[MenuButton]: # used in aiotgm.__init__
-    '''
-    Function to deserialize MenuButton.
+class ShippingAddress(TelegramType):
     '''
-    if res is None: return None
-    obj = _check_dict(res)
-
-    type = obj.pop('type')
-
-    if type == DEFAULT_MENU_BUTTON_COMMANDS:
-        return MenuButtonCommands._dese(obj, check_dict=False)
-
-    elif type == DEFAULT_MENU_BUTTON_WEB_APP:
-        return MenuButtonWebApp._dese(obj, check_dict=False)
-
-    elif type == DEFAULT_MENU_BUTTON_DEFAULT:
-        return MenuButtonDefault._dese(obj, check_dict=False)
-    else:
-        raise ValueError(
-            'An error occurred during the deserialization'
-            f' of the type MenuButton. Invalid type: {type!r}.'
-        )
-
-# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
+    https://core.telegram.org/bots/api#shippingaddress
 
-class ResponseParameters(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#responseparameters
+    This object represents a shipping address.
 
-    Describes why a request was unsuccessful.
+    :param country_code: Two-letter `ISO 3166-1 alpha-2 <https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2>`_ country code.
+    :type country_code: :obj:`str`
+    :param state: State, if applicable.
+    :type state: :obj:`str`
+    :param city: City.
+    :type city: :obj:`str`
+    :param street_line1: First line for the address.
+    :type street_line1: :obj:`str`
+    :param street_line2: Second line for the address.
+    :type street_line2: :obj:`str`
+    :param post_code: Address post code.
+    :type post_code: :obj:`str`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['migrate_to_chat_id'] = res.get('migrate_to_chat_id')
-        obj['retry_after'] = res.get('retry_after')
+        obj['country_code'] = res.get('country_code')
+        obj['state'] = res.get('state')
+        obj['city'] = res.get('city')
+        obj['street_line1'] = res.get('street_line1')
+        obj['street_line2'] = res.get('street_line2')
+        obj['post_code'] = res.get('post_code')
         return cls(**obj)
 
     def __init__(
         self,
-        migrate_to_chat_id: Optional[int] = None,
-        retry_after: Optional[int] = None
+        country_code: str,
+        state: str,
+        city: str,
+        street_line1: str,
+        street_line2: str,
+        post_code: str
     ):
-        self.migrate_to_chat_id = migrate_to_chat_id
-        self.retry_after = retry_after
+        self.country_code = country_code
+        self.state = state
+        self.city = city
+        self.street_line1 = street_line1
+        self.street_line2 = street_line2
+        self.post_code = post_code
 
 
-class MaskPosition(TelegramType):
+class ShippingOption(TelegramType):
     '''
-    https://core.telegram.org/bots/api#maskposition
+    https://core.telegram.org/bots/api#shippingoption
 
-    This object describes the position on faces where a mask should be placed by default.
+    This object represents one shipping option.
+
+    :param id: Shipping option identifier.
+    :type id: :obj:`str`
+    :param title: Option title.
+    :type title: :obj:`str`
+    :param prices: List of price portions.
+    :type prices: :obj:`list` of :obj:`~aiotgm.types.LabeledPrice`
+    '''
+    def __init__(
+        self,
+        id: str,
+        title: str,
+        prices: list[LabeledPrice]
+    ):
+        self.id = id
+        self.title = title
+        self.prices = prices
+
+
+class ShippingQuery(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#shippingquery
+
+    This object contains information about an incoming shipping query.
+
+    :param id: Unique query identifier.
+    :type id: :obj:`str`
+    :param from_user: User who sent the query.
+    :type from_user: :obj:`~aiotgm.types.User`
+    :param invoice_payload: Bot specified invoice payload.
+    :type invoice_payload: :obj:`str`
+    :param shipping_address: User specified shipping address.
+    :type shipping_address: :obj:`~aiotgm.types.ShippingAddress`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['point'] = res.get('point')
-        obj['x_shift'] = res.get('x_shift')
-        obj['y_shift'] = res.get('y_shift')
-        obj['scale'] = res.get('scale')
+        obj['id'] = res.get('id')
+        obj['from_user'] = User._dese(res.get('from_user'))
+        obj['invoice_payload'] = res.get('invoice_payload')
+        obj['shipping_address'] = ShippingAddress._dese(res.get('shipping_address'))
         return cls(**obj)
 
     def __init__(
         self,
-        point: str,
-        x_shift: float,
-        y_shift: float,
-        scale: float
+        id: str,
+        from_user: User,
+        invoice_payload: str,
+        shipping_address: ShippingAddress
     ):
-        self.point = point
-        self.x_shift = x_shift
-        self.y_shift = y_shift
-        self.scale = scale
+        self.id = id
+        self.from_user = from_user
+        self.invoice_payload = invoice_payload
+        self.shipping_address = shipping_address
 
 
 class Sticker(TelegramType):
     '''
     https://core.telegram.org/bots/api#sticker
 
     This object represents a sticker.
+
+    :param file_id: Identifier for this file, which can be used to download or reuse the file.
+    :type file_id: :obj:`str`
+    :param file_unique_id: Unique identifier for this file, which is supposed to be the same over time and for different bots. Can't be used to download or reuse the file.
+    :type file_unique_id: :obj:`str`
+    :param type: Type of the sticker, currently one of “regular”, “mask”, “custom_emoji”. The type of the sticker is independent from its format, which is determined by the fields *is_animated* and *is_video*.
+    :type type: :obj:`str`
+    :param width: Sticker width.
+    :type width: :obj:`int`
+    :param height: Sticker height.
+    :type height: :obj:`int`
+    :param is_animated: :obj:`True`, if the sticker is `animated <https://telegram.org/blog/animated-stickers>`_.
+    :type is_animated: :obj:`bool`
+    :param is_video: :obj:`True`, if the sticker is a `video sticker <https://telegram.org/blog/video-stickers-better-reactions>`_.
+    :type is_video: :obj:`bool`
+    :param thumbnail: Sticker thumbnail in the .WEBP or .JPG format.
+    :type thumbnail: :obj:`~aiotgm.types.PhotoSize`, optional
+    :param emoji: Emoji associated with the sticker.
+    :type emoji: :obj:`str`, optional
+    :param set_name: Name of the sticker set to which the sticker belongs.
+    :type set_name: :obj:`str`, optional
+    :param premium_animation: For premium regular stickers, premium animation for the sticker.
+    :type premium_animation: :obj:`~aiotgm.types.File`, optional
+    :param mask_position: For mask stickers, the position where the mask should be placed.
+    :type mask_position: :obj:`~aiotgm.types.MaskPosition`, optional
+    :param custom_emoji_id: For custom emoji stickers, unique identifier of the custom emoji.
+    :type custom_emoji_id: :obj:`str`, optional
+    :param needs_repainting: :obj:`True`, if the sticker must be repainted to a text color in messages, the color of the Telegram Premium badge in emoji status, white color on chat photos, or another appropriate color in other places.
+    :type needs_repainting: :obj:`True`, optional
+    :param file_size: File size in bytes.
+    :type file_size: :obj:`int`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
         obj['file_id'] = res.get('file_id')
         obj['file_unique_id'] = res.get('file_unique_id')
@@ -6535,14 +7222,25 @@
 
 
 class StickerSet(TelegramType):
     '''
     https://core.telegram.org/bots/api#stickerset
 
     This object represents a sticker set.
+
+    :param name: Sticker set name.
+    :type name: :obj:`str`
+    :param title: Sticker set title.
+    :type title: :obj:`str`
+    :param sticker_type: Type of stickers in the set, currently one of “regular”, “mask”, “custom_emoji”.
+    :type sticker_type: :obj:`str`
+    :param stickers: List of all set stickers.
+    :type stickers: :obj:`list` of :obj:`~aiotgm.types.Sticker`
+    :param thumbnail: Sticker set thumbnail in the .WEBP, .TGS, or .WEBM format.
+    :type thumbnail: :obj:`~aiotgm.types.PhotoSize`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
         obj['name'] = res.get('name')
         obj['title'] = res.get('title')
@@ -6562,889 +7260,860 @@
         self.name = name
         self.title = title
         self.sticker_type = sticker_type
         self.stickers = stickers
         self.thumbnail = thumbnail
 
 
-class InputSticker(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#inputsticker
-
-    This object describes a sticker to be added to a sticker set.
-    '''
-    def __init__(
-        self,
-        sticker: Union[InputFile, str],
-        format: str,
-        emoji_list: list[str],
-        mask_position: Optional[MaskPosition] = None,
-        keywords: Optional[list[str]] = None
-    ):
-        self.sticker = sticker
-        self.format = format
-        self.emoji_list = emoji_list
-        self.mask_position = mask_position
-        self.keywords = keywords
-
-
-class InputTextMessageContent(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#inputtextmessagecontent
-
-    Represents the content of a text message to be sent as the result of an inline query.
-    '''
-    def __init__(
-        self,
-        message_text: str,
-        parse_mode: Optional[str] = None,
-        entities: Optional[list[MessageEntity]] = None,
-        link_preview_options: Optional[LinkPreviewOptions] = None
-    ):
-        self.message_text = message_text
-        self.parse_mode = parse_mode
-        self.entities = entities
-        self.link_preview_options = link_preview_options
-
-
-class InputVenueMessageContent(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#inputvenuemessagecontent
-
-    Represents the content of a venue message to be sent as the result of an inline query.
+class Story(TelegramType):
     '''
-    def __init__(
-        self,
-        latitude: float,
-        longitude: float,
-        title: str,
-        address: str,
-        foursquare_id: Optional[str] = None,
-        foursquare_type: Optional[str] = None,
-        google_place_id: Optional[str] = None,
-        google_place_type: Optional[str] = None
-    ):
-        self.latitude = latitude
-        self.longitude = longitude
-        self.title = title
-        self.address = address
-        self.foursquare_id = foursquare_id
-        self.foursquare_type = foursquare_type
-        self.google_place_id = google_place_id
-        self.google_place_type = google_place_type
-
+    https://core.telegram.org/bots/api#story
 
-class SentWebAppMessage(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#sentwebappmessage
+    This object represents a story.
 
-    Describes an inline message sent by a Web App on behalf of a user.
+    :param chat: Chat that posted the story.
+    :type chat: :obj:`~aiotgm.types.Chat`
+    :param id: Unique identifier for the story in the chat.
+    :type id: :obj:`int`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['inline_message_id'] = res.get('inline_message_id')
+        obj['chat'] = Chat._dese(res.get('chat'))
+        obj['id'] = res.get('id')
         return cls(**obj)
 
     def __init__(
         self,
-        inline_message_id: Optional[str] = None
+        chat: Chat,
+        id: int
     ):
-        self.inline_message_id = inline_message_id
+        self.chat = chat
+        self.id = id
 
 
-class Invoice(TelegramType):
+class SuccessfulPayment(TelegramType):
     '''
-    https://core.telegram.org/bots/api#invoice
+    https://core.telegram.org/bots/api#successfulpayment
 
-    This object contains basic information about an invoice.
+    This object contains basic information about a successful payment.
+
+    :param currency: Three-letter ISO 4217 `currency <https://core.telegram.org/bots/payments#supported-currencies>`_ code.
+    :type currency: :obj:`str`
+    :param total_amount: Total price in the *smallest units* of the currency (integer, **not** float/double). For example, for a price of ``US$ 1.45`` pass ``amount = 145``. See the *exp* parameter in `currencies.json <https://core.telegram.org/bots/payments/currencies.json>`_, it shows the number of digits past the decimal point for each currency (2 for the majority of currencies).
+    :type total_amount: :obj:`int`
+    :param invoice_payload: Bot specified invoice payload.
+    :type invoice_payload: :obj:`str`
+    :param telegram_payment_charge_id: Telegram payment identifier.
+    :type telegram_payment_charge_id: :obj:`str`
+    :param provider_payment_charge_id: Provider payment identifier.
+    :type provider_payment_charge_id: :obj:`str`
+    :param shipping_option_id: Identifier of the shipping option chosen by the user.
+    :type shipping_option_id: :obj:`str`, optional
+    :param order_info: Order information provided by the user.
+    :type order_info: :obj:`~aiotgm.types.OrderInfo`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['title'] = res.get('title')
-        obj['description'] = res.get('description')
-        obj['start_parameter'] = res.get('start_parameter')
         obj['currency'] = res.get('currency')
         obj['total_amount'] = res.get('total_amount')
+        obj['invoice_payload'] = res.get('invoice_payload')
+        obj['shipping_option_id'] = res.get('shipping_option_id')
+        obj['order_info'] = OrderInfo._dese(res.get('order_info'))
+        obj['telegram_payment_charge_id'] = res.get('telegram_payment_charge_id')
+        obj['provider_payment_charge_id'] = res.get('provider_payment_charge_id')
         return cls(**obj)
 
     def __init__(
         self,
-        title: str,
-        description: str,
-        start_parameter: str,
         currency: str,
-        total_amount: int
+        total_amount: int,
+        invoice_payload: str,
+        telegram_payment_charge_id: str,
+        provider_payment_charge_id: str,
+        shipping_option_id: Optional[str] = None,
+        order_info: Optional[OrderInfo] = None
     ):
-        self.title = title
-        self.description = description
-        self.start_parameter = start_parameter
         self.currency = currency
         self.total_amount = total_amount
+        self.invoice_payload = invoice_payload
+        self.telegram_payment_charge_id = telegram_payment_charge_id
+        self.provider_payment_charge_id = provider_payment_charge_id
+        self.shipping_option_id = shipping_option_id
+        self.order_info = order_info
 
 
-class ShippingAddress(TelegramType):
+class SwitchInlineQueryChosenChat(TelegramType):
     '''
-    https://core.telegram.org/bots/api#shippingaddress
+    https://core.telegram.org/bots/api#switchinlinequerychosenchat
 
-    This object represents a shipping address.
+    This object represents an inline button that switches the current user
+    to inline mode in a chosen chat, with an optional default inline query.
+
+    :param query: The default inline query to be inserted in the input field. If left empty, only the bot's username will be inserted.
+    :type query: :obj:`str`, optional
+    :param allow_user_chats: :obj:`True`, if private chats with users can be chosen.
+    :type allow_user_chats: :obj:`bool`, optional
+    :param allow_bot_chats: :obj:`True`, if private chats with bots can be chosen.
+    :type allow_bot_chats: :obj:`bool`, optional
+    :param allow_group_chats: :obj:`True`, if group and supergroup chats can be chosen.
+    :type allow_group_chats: :obj:`bool`, optional
+    :param allow_channel_chats: :obj:`True`, if channel chats can be chosen.
+    :type allow_channel_chats: :obj:`bool`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['country_code'] = res.get('country_code')
-        obj['state'] = res.get('state')
-        obj['city'] = res.get('city')
-        obj['street_line1'] = res.get('street_line1')
-        obj['street_line2'] = res.get('street_line2')
-        obj['post_code'] = res.get('post_code')
+        obj['query'] = res.get('query')
+        obj['allow_user_chats'] = res.get('allow_user_chats')
+        obj['allow_bot_chats'] = res.get('allow_bot_chats')
+        obj['allow_group_chats'] = res.get('allow_group_chats')
+        obj['allow_channel_chats'] = res.get('allow_channel_chats')
         return cls(**obj)
 
     def __init__(
         self,
-        country_code: str,
-        state: str,
-        city: str,
-        street_line1: str,
-        street_line2: str,
-        post_code: str
+        query: Optional[str] = None,
+        allow_user_chats: Optional[bool] = None,
+        allow_bot_chats: Optional[bool] = None,
+        allow_group_chats: Optional[bool] = None,
+        allow_channel_chats: Optional[bool] = None
     ):
-        self.country_code = country_code
-        self.state = state
-        self.city = city
-        self.street_line1 = street_line1
-        self.street_line2 = street_line2
-        self.post_code = post_code
+        self.query = query
+        self.allow_user_chats = allow_user_chats
+        self.allow_bot_chats = allow_bot_chats
+        self.allow_group_chats = allow_group_chats
+        self.allow_channel_chats = allow_channel_chats
 
 
-class OrderInfo(TelegramType):
+class TextQuote(TelegramType):
     '''
-    https://core.telegram.org/bots/api#orderinfo
+    https://core.telegram.org/bots/api#textquote
 
-    This object represents information about an order.
+    This object contains information about the quoted part
+    of a message that is replied to by the given message.
+
+    :param text: Text of the quoted part of a message that is replied to by the given message.
+    :type text: :obj:`str`
+    :param position: Approximate quote position in the original message in UTF-16 code units as specified by the sender.
+    :type position: :obj:`int`
+    :param entities: Special entities that appear in the quote. Currently, only *bold*, *italic*, *underline*, *strikethrough*, *spoiler*, and *custom_emoji entities* are kept in quotes.
+    :type entities: :obj:`list` of :obj:`~aiotgm.types.MessageEntity`, optional
+    :param is_manual: :obj:`True`, if the quote was chosen manually by the message sender. Otherwise, the quote was added automatically by the server.
+    :type is_manual: :obj:`True`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['name'] = res.get('name')
-        obj['phone_number'] = res.get('phone_number')
-        obj['email'] = res.get('email')
-        obj['shipping_address'] = ShippingAddress._dese(res.get('shipping_address'))
+        obj['text'] = res.get('text')
+        obj['position'] = res.get('position')
+        obj['entities'] = [MessageEntity._dese(kwargs) for kwargs in res.get('entities')] if 'entities' in res else None
+        obj['is_manual'] = res.get('is_manual')
         return cls(**obj)
 
     def __init__(
         self,
-        name: Optional[str] = None,
-        phone_number: Optional[str] = None,
-        email: Optional[str] = None,
-        shipping_address: Optional[ShippingAddress] = None
+        text: str,
+        position: int,
+        entities: Optional[list[MessageEntity]] = None,
+        is_manual: Optional[Literal[True]] = None
     ):
-        self.name = name
-        self.phone_number = phone_number
-        self.email = email
-        self.shipping_address = shipping_address
+        self.text = text
+        self.position = position
+        self.entities = entities
+        self.is_manual = is_manual
 
 
-class ShippingOption(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#shippingoption
-
-    This object represents one shipping option.
+class Update(TelegramType):
     '''
-    def __init__(
-        self,
-        id: str,
-        title: str,
-        prices: list[LabeledPrice]
-    ):
-        self.id = id
-        self.title = title
-        self.prices = prices
-
+    https://core.telegram.org/bots/api#update
 
-class SuccessfulPayment(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#successfulpayment
+    This `object <https://core.telegram.org/bots/api#available-types>`_ represents an
+    incoming update. At most one of the optional parameters can be present in any given update.
 
-    This object contains basic information about a successful payment.
+    :param update_id: The update's unique identifier. Update identifiers start from a certain positive number and increase sequentially. This identifier becomes especially handy if you're using `webhooks <https://core.telegram.org/bots/api#setwebhook>`_, since it allows you to ignore repeated updates or to restore the correct update sequence, should they get out of order. If there are no new updates for at least a week, then identifier of the next update will be chosen randomly instead of sequentially.
+    :type update_id: :obj:`int`
+    :param message: New incoming message of any kind - text, photo, sticker, etc.
+    :type message: :obj:`~aiotgm.types.Message`, optional
+    :param edited_message: New version of a message that is known to the bot and was edited. This update may at times be triggered by changes to message fields that are either unavailable or not actively used by your bot.
+    :type edited_message: :obj:`~aiotgm.types.Message`, optional
+    :param channel_post: New incoming channel post of any kind - text, photo, sticker, etc.
+    :type channel_post: :obj:`~aiotgm.types.Message`, optional
+    :param edited_channel_post: New version of a channel post that is known to the bot and was edited. This update may at times be triggered by changes to message fields that are either unavailable or not actively used by your bot.
+    :type edited_channel_post: :obj:`~aiotgm.types.Message`, optional
+    :param business_connection: The bot was connected to or disconnected from a business account, or a user edited an existing connection with the bot.
+    :type business_connection: :obj:`~aiotgm.types.BusinessConnection`, optional
+    :param business_message: New non-service message from a connected business account.
+    :type business_message: :obj:`~aiotgm.types.Message`, optional
+    :param edited_business_message: New version of a message from a connected business account.
+    :type edited_business_message: :obj:`~aiotgm.types.Message`, optional
+    :param deleted_business_messages: Messages were deleted from a connected business account.
+    :type deleted_business_messages: :obj:`~aiotgm.types.BusinessMessagesDeleted`, optional
+    :param message_reaction: A reaction to a message was changed by a user. The bot must be an administrator in the chat and must explicitly specify ``"message_reaction"`` in the list of *allowed_updates* to receive these updates. The update isn't received for reactions set by bots.
+    :type message_reaction: :obj:`~aiotgm.types.MessageReactionUpdated`, optional
+    :param message_reaction_count: Reactions to a message with anonymous reactions were changed. The bot must be an administrator in the chat and must explicitly specify ``"message_reaction_count"`` in the list of *allowed_updates* to receive these updates. The updates are grouped and can be sent with delay up to a few minutes.
+    :type message_reaction_count: :obj:`~aiotgm.types.MessageReactionCountUpdated`, optional
+    :param inline_query: New incoming `inline <https://core.telegram.org/bots/api#inline-mode>`_ query.
+    :type inline_query: :obj:`~aiotgm.types.InlineQuery`, optional
+    :param chosen_inline_result: The result of an `inline <https://core.telegram.org/bots/api#inline-mode>`_ query that was chosen by a user and sent to their chat partner. Please see our documentation on the `feedback collecting <https://core.telegram.org/bots/inline#collecting-feedback>`_ for details on how to enable these updates for your bot.
+    :type chosen_inline_result: :obj:`~aiotgm.types.ChosenInlineResult`, optional
+    :param callback_query: New incoming callback query.
+    :type callback_query: :obj:`~aiotgm.types.CallbackQuery`, optional
+    :param shipping_query: New incoming shipping query. Only for invoices with flexible price.
+    :type shipping_query: :obj:`~aiotgm.types.ShippingQuery`, optional
+    :param pre_checkout_query: New incoming pre-checkout query. Contains full information about checkout.
+    :type pre_checkout_query: :obj:`~aiotgm.types.PreCheckoutQuery`, optional
+    :param poll: New poll state. Bots receive only updates about manually stopped polls and polls, which are sent by the bot.
+    :type poll: :obj:`~aiotgm.types.Poll`, optional
+    :param poll_answer: A user changed their answer in a non-anonymous poll. Bots receive new votes only in polls that were sent by the bot itself.
+    :type poll_answer: :obj:`~aiotgm.types.PollAnswer`, optional
+    :param my_chat_member: The bot's chat member status was updated in a chat. For private chats, this update is received only when the bot is blocked or unblocked by the user.
+    :type my_chat_member: :obj:`~aiotgm.types.ChatMemberUpdated`, optional
+    :param chat_member: A chat member's status was updated in a chat. The bot must be an administrator in the chat and must explicitly specify ``"chat_member"`` in the list of *allowed_updates* to receive these updates.
+    :type chat_member: :obj:`~aiotgm.types.ChatMemberUpdated`, optional
+    :param chat_join_request: A request to join the chat has been sent. The bot must have the *can_invite_users* administrator right in the chat to receive these updates.
+    :type chat_join_request: :obj:`~aiotgm.types.ChatJoinRequest`, optional
+    :param chat_boost: A chat boost was added or changed. The bot must be an administrator in the chat to receive these updates.
+    :type chat_boost: :obj:`~aiotgm.types.ChatBoostUpdated`, optional
+    :param removed_chat_boost: A boost was removed from a chat. The bot must be an administrator in the chat to receive these updates.
+    :type removed_chat_boost: :obj:`~aiotgm.types.ChatBoostRemoved`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['currency'] = res.get('currency')
-        obj['total_amount'] = res.get('total_amount')
-        obj['invoice_payload'] = res.get('invoice_payload')
-        obj['shipping_option_id'] = res.get('shipping_option_id')
-        obj['order_info'] = OrderInfo._dese(res.get('order_info'))
-        obj['telegram_payment_charge_id'] = res.get('telegram_payment_charge_id')
-        obj['provider_payment_charge_id'] = res.get('provider_payment_charge_id')
+        obj['update_id'] = res.get('update_id')
+        obj['message'] = Message._dese(res.get('message'))
+        obj['edited_message'] = Message._dese(res.get('edited_message'))
+        obj['channel_post'] = Message._dese(res.get('channel_post'))
+        obj['edited_channel_post'] = Message._dese(res.get('edited_channel_post'))
+        obj['business_connection'] = BusinessConnection._dese(res.get('business_connection'))
+        obj['business_message'] = Message._dese(res.get('business_message'))
+        obj['edited_business_message'] = Message._dese(res.get('edited_business_message'))
+        obj['deleted_business_messages'] = BusinessMessagesDeleted._dese(res.get('deleted_business_messages'))
+        obj['message_reaction'] = MessageReactionUpdated._dese(res.get('message_reaction'))
+        obj['message_reaction_count'] = MessageReactionCountUpdated._dese(res.get('message_reaction_count'))
+        obj['inline_query'] = InlineQuery._dese(res.get('inline_query'))
+        obj['chosen_inline_result'] = ChosenInlineResult._dese(res.get('chosen_inline_result'))
+        obj['callback_query'] = CallbackQuery._dese(res.get('callback_query'))
+        obj['shipping_query'] = ShippingQuery._dese(res.get('shipping_query'))
+        obj['pre_checkout_query'] = PreCheckoutQuery._dese(res.get('pre_checkout_query'))
+        obj['poll'] = Poll._dese(res.get('poll'))
+        obj['poll_answer'] = PollAnswer._dese(res.get('poll_answer'))
+        obj['my_chat_member'] = ChatMemberUpdated._dese(res.get('my_chat_member'))
+        obj['chat_member'] = ChatMemberUpdated._dese(res.get('chat_member'))
+        obj['chat_join_request'] = ChatJoinRequest._dese(res.get('chat_join_request'))
+        obj['chat_boost'] = ChatBoostUpdated._dese(res.get('chat_boost'))
+        obj['removed_chat_boost'] = ChatBoostRemoved._dese(res.get('removed_chat_boost'))
         return cls(**obj)
 
     def __init__(
         self,
-        currency: str,
-        total_amount: int,
-        invoice_payload: str,
-        telegram_payment_charge_id: str,
-        provider_payment_charge_id: str,
-        shipping_option_id: Optional[str] = None,
-        order_info: Optional[OrderInfo] = None
+        update_id: int,
+        message: Optional[Message] = None,
+        edited_message: Optional[Message] = None,
+        channel_post: Optional[Message] = None,
+        edited_channel_post: Optional[Message] = None,
+        business_connection: Optional[BusinessConnection] = None,
+        business_message: Optional[Message] = None,
+        edited_business_message: Optional[Message] = None,
+        deleted_business_messages: Optional[BusinessMessagesDeleted] = None,
+        message_reaction: Optional[MessageReactionUpdated] = None,
+        message_reaction_count: Optional[MessageReactionCountUpdated] = None,
+        inline_query: Optional[InlineQuery] = None,
+        chosen_inline_result: Optional[ChosenInlineResult] = None,
+        callback_query: Optional[CallbackQuery] = None,
+        shipping_query: Optional[ShippingQuery] = None,
+        pre_checkout_query: Optional[PreCheckoutQuery] = None,
+        poll: Optional[Poll] = None,
+        poll_answer: Optional[PollAnswer] = None,
+        my_chat_member: Optional[ChatMemberUpdated] = None,
+        chat_member: Optional[ChatMemberUpdated] = None,
+        chat_join_request: Optional[ChatJoinRequest] = None,
+        chat_boost: Optional[ChatBoostUpdated] = None,
+        removed_chat_boost: Optional[ChatBoostRemoved] = None
     ):
-        self.currency = currency
-        self.total_amount = total_amount
-        self.invoice_payload = invoice_payload
-        self.telegram_payment_charge_id = telegram_payment_charge_id
-        self.provider_payment_charge_id = provider_payment_charge_id
-        self.shipping_option_id = shipping_option_id
-        self.order_info = order_info
+        self.update_id = update_id
+        self.message = message
+        self.edited_message = edited_message
+        self.channel_post = channel_post
+        self.edited_channel_post = edited_channel_post
+        self.business_connection = business_connection
+        self.business_message = business_message
+        self.edited_business_message = edited_business_message
+        self.deleted_business_messages = deleted_business_messages
+        self.message_reaction = message_reaction
+        self.message_reaction_count = message_reaction_count
+        self.inline_query = inline_query
+        self.chosen_inline_result = chosen_inline_result
+        self.callback_query = callback_query
+        self.shipping_query = shipping_query
+        self.pre_checkout_query = pre_checkout_query
+        self.poll = poll
+        self.poll_answer = poll_answer
+        self.my_chat_member = my_chat_member
+        self.chat_member = chat_member
+        self.chat_join_request = chat_join_request
+        self.chat_boost = chat_boost
+        self.removed_chat_boost = removed_chat_boost
 
 
-class ShippingQuery(TelegramType):
+class User(TelegramType):
     '''
-    https://core.telegram.org/bots/api#shippingquery
+    https://core.telegram.org/bots/api#user
 
-    This object contains information about an incoming shipping query.
+    This object represents a Telegram user or bot.
+
+    :param id: Unique identifier for this user or bot. This number may have more than 32 significant bits and some programming languages may have difficulty/silent defects in interpreting it. But it has at most 52 significant bits, so a 64-bit integer or double-precision float type are safe for storing this identifier.
+    :type id: :obj:`int`
+    :param is_bot: :obj:`True`, if this user is a bot.
+    :type is_bot: :obj:`bool`
+    :param first_name: User's or bot's first name.
+    :type first_name: :obj:`str`
+    :param last_name: User's or bot's last name.
+    :type last_name: :obj:`str`, optional
+    :param username: User's or bot's username.
+    :type username: :obj:`str`, optional
+    :param language_code: `IETF language tag <https://en.wikipedia.org/wiki/IETF_language_tag>`_ of the user's language.
+    :type language_code: :obj:`str`, optional
+    :param is_premium: :obj:`True`, if this user is a Telegram Premium user.
+    :type is_premium: :obj:`True`, optional
+    :param added_to_attachment_menu: :obj:`True`, if this user added the bot to the attachment menu.
+    :type added_to_attachment_menu: :obj:`True`, optional
+    :param can_join_groups: :obj:`True`, if the bot can be invited to groups. Returned only in :meth:`~aiotgm.Client.get_me`.
+    :type can_join_groups: :obj:`bool`, optional
+    :param can_read_all_group_messages: :obj:`True`, if privacy mode is disabled for the bot. Returned only in :meth:`~aiotgm.Client.get_me`.
+    :type can_read_all_group_messages: :obj:`bool`, optional
+    :param supports_inline_queries: :obj:`True`, if the bot supports inline queries. Returned only in :meth:`~aiotgm.Client.get_me`.
+    :type supports_inline_queries: :obj:`bool`, optional
+    :param can_connect_to_business: :obj:`True`, if the bot can be connected to a Telegram Business account to receive its messages. Returned only in :meth:`~aiotgm.Client.get_me`.
+    :type can_connect_to_business: :obj:`bool`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
         obj['id'] = res.get('id')
-        obj['from_user'] = User._dese(res.get('from_user'))
-        obj['invoice_payload'] = res.get('invoice_payload')
-        obj['shipping_address'] = ShippingAddress._dese(res.get('shipping_address'))
+        obj['is_bot'] = res.get('is_bot')
+        obj['first_name'] = res.get('first_name')
+        obj['last_name'] = res.get('last_name')
+        obj['username'] = res.get('username')
+        obj['language_code'] = res.get('language_code')
+        obj['is_premium'] = res.get('is_premium')
+        obj['added_to_attachment_menu'] = res.get('added_to_attachment_menu')
+        obj['can_join_groups'] = res.get('can_join_groups')
+        obj['can_read_all_group_messages'] = res.get('can_read_all_group_messages')
+        obj['supports_inline_queries'] = res.get('supports_inline_queries')
+        obj['can_connect_to_business'] = res.get('can_connect_to_business')
         return cls(**obj)
 
     def __init__(
         self,
-        id: str,
-        from_user: User,
-        invoice_payload: str,
-        shipping_address: ShippingAddress
+        id: int,
+        is_bot: bool,
+        first_name: str,
+        last_name: Optional[str] = None,
+        username: Optional[str] = None,
+        language_code: Optional[str] = None,
+        is_premium: Optional[Literal[True]] = None,
+        added_to_attachment_menu: Optional[Literal[True]] = None,
+        can_join_groups: Optional[bool] = None,
+        can_read_all_group_messages: Optional[bool] = None,
+        supports_inline_queries: Optional[bool] = None,
+        can_connect_to_business: Optional[bool] = None
     ):
         self.id = id
-        self.from_user = from_user
-        self.invoice_payload = invoice_payload
-        self.shipping_address = shipping_address
+        self.is_bot = is_bot
+        self.first_name = first_name
+        self.last_name = last_name
+        self.username = username
+        self.language_code = language_code
+        self.is_premium = is_premium
+        self.added_to_attachment_menu = added_to_attachment_menu
+        self.can_join_groups = can_join_groups
+        self.can_read_all_group_messages = can_read_all_group_messages
+        self.supports_inline_queries = supports_inline_queries
+        self.can_connect_to_business = can_connect_to_business
 
 
-class PreCheckoutQuery(TelegramType):
+class UserChatBoosts(TelegramType):
     '''
-    https://core.telegram.org/bots/api#precheckoutquery
+    https://core.telegram.org/bots/api#userchatboosts
 
-    This object contains information about an incoming pre-checkout query.
+    This object represents a list of boosts added to a chat by a user.
+
+    :param boosts: The list of boosts added to the chat by the user.
+    :type boosts: :obj:`list` of :obj:`~aiotgm.types.ChatBoost`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['id'] = res.get('id')
-        obj['from_user'] = User._dese(res.get('from_user'))
-        obj['currency'] = res.get('currency')
-        obj['total_amount'] = res.get('total_amount')
-        obj['invoice_payload'] = res.get('invoice_payload')
-        obj['shipping_option_id'] = res.get('shipping_option_id')
-        obj['order_info'] = OrderInfo._dese(res.get('order_info'))
+        obj['boosts'] = [ChatBoost._dese(kwargs) for kwargs in res.get('boosts')]
         return cls(**obj)
 
     def __init__(
         self,
-        id: str,
-        from_user: User,
-        currency: str,
-        total_amount: int,
-        invoice_payload: str,
-        shipping_option_id: Optional[str] = None,
-        order_info: Optional[OrderInfo] = None
+        boosts: list[ChatBoost]
     ):
-        self.id = id
-        self.from_user = from_user
-        self.currency = currency
-        self.total_amount = total_amount
-        self.invoice_payload = invoice_payload
-        self.shipping_option_id = shipping_option_id
-        self.order_info = order_info
+        self.boosts = boosts
 
 
-class PassportFile(TelegramType):
+class UserProfilePhotos(TelegramType):
     '''
-    https://core.telegram.org/bots/api#passportfile
+    https://core.telegram.org/bots/api#userprofilephotos
 
-    This object represents a file uploaded to Telegram Passport.\n
-    Currently all Telegram Passport files are in JPEG format when decrypted and don't exceed 10MB.
+    This object represent a user's profile pictures.
+
+    :param total_count: Total number of profile pictures the target user has.
+    :type total_count: :obj:`int`
+    :param photos: Requested profile pictures (in up to 4 sizes each).
+    :type photos: :obj:`list` of :obj:`list` of :obj:`~aiotgm.types.PhotoSize`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['file_id'] = res.get('file_id')
-        obj['file_unique_id'] = res.get('file_unique_id')
-        obj['file_size'] = res.get('file_size')
-        obj['file_date'] = res.get('file_date')
+        obj['total_count'] = res.get('total_count')
+        obj['photos'] = [[PhotoSize._dese(kwargs) for kwargs in lst] for lst in res.get('photos')]
         return cls(**obj)
 
     def __init__(
         self,
-        file_id: str,
-        file_unique_id: str,
-        file_size: int,
-        file_date: int
+        total_count: int,
+        photos: list[list[PhotoSize]]
     ):
-        self.file_id = file_id
-        self.file_unique_id = file_unique_id
-        self.file_size = file_size
-        self.file_date = file_date
+        self.total_count = total_count
+        self.photos = photos
 
 
-class PassportData(TelegramType):
+class UsersShared(TelegramType):
     '''
-    https://core.telegram.org/bots/api#passportdata
+    https://core.telegram.org/bots/api#usersshared
 
-    Describes Telegram Passport data shared with the bot by the user.
+    This object contains information about the users whose identifiers
+    were shared with the bot using a :obj:`~aiotgm.types.KeyboardButtonRequestUsers` button.
+
+    :param request_id: Identifier of the request.
+    :type request_id: :obj:`int`
+    :param users: Information about users shared with the bot.
+    :type users: :obj:`list` of :obj:`~aiotgm.types.SharedUser`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['data'] = [EncryptedPassportElement._dese(kwargs) for kwargs in res.get('data')]
-        obj['credentials'] = EncryptedCredentials._dese(res.get('credentials'))
+        obj['request_id'] = res.get('request_id')
+        obj['users'] = [SharedUser._dese(kwargs) for kwargs in res.get('users')]
         return cls(**obj)
 
     def __init__(
         self,
-        data: list[EncryptedPassportElement],
-        credentials: EncryptedCredentials
+        request_id: int,
+        users: list[SharedUser]
     ):
-        self.data = data
-        self.credentials = credentials
-
-
-# PassportElementError: 9 SUBCLASSES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        self.request_id = request_id
+        self.users = users
 
-class PassportElementErrorDataField(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#passportelementerrordatafield
 
-    Represents an issue in one of the data fields that was provided by the user.\n
-    The error is considered resolved when the field's value changes.
+class Venue(TelegramType):
     '''
-    def __init__(
-        self,
-        type: Literal[
-            'personal_details',
-            'passport',
-            'driver_license',
-            'identity_card',
-            'internal_passport',
-            'address'
-        ],
-        field_name: str,
-        data_hash: str,
-        message: str
-    ):
-        self.source = DEFAULT_PASSPORT_ELEMENT_ERROR_DATA_FIELD
-        self.type = type
-        self.field_name = field_name
-        self.data_hash = data_hash
-        self.message = message
+    https://core.telegram.org/bots/api#venue
 
+    This object represents a venue.
 
-class PassportElementErrorFrontSide(TelegramType):
+    :param location: Venue location. Can't be a live location.
+    :type location: :obj:`~aiotgm.types.Location`
+    :param title: Name of the venue.
+    :type title: :obj:`str`
+    :param address: Address of the venue.
+    :type address: :obj:`str`
+    :param foursquare_id: Foursquare identifier of the venue.
+    :type foursquare_id: :obj:`str`, optional
+    :param foursquare_type: Foursquare type of the venue. (For example, “arts_entertainment/default”, “arts_entertainment/aquarium” or “food/icecream”.)
+    :type foursquare_type: :obj:`str`, optional
+    :param google_place_id: Google Places identifier of the venue.
+    :type google_place_id: :obj:`str`, optional
+    :param google_place_type: Google Places type of the venue. (See `supported types <https://developers.google.com/places/web-service/supported_types>`_.)
+    :type google_place_type: :obj:`str`, optional
     '''
-    https://core.telegram.org/bots/api#passportelementerrorfrontside
+    @classmethod
+    @_parse_result
+    def _dese(cls, res: dict):
+        obj = {}
+        obj['location'] = Location._dese(res.get('location'))
+        obj['title'] = res.get('title')
+        obj['address'] = res.get('address')
+        obj['foursquare_id'] = res.get('foursquare_id')
+        obj['foursquare_type'] = res.get('foursquare_type')
+        obj['google_place_id'] = res.get('google_place_id')
+        obj['google_place_type'] = res.get('google_place_type')
+        return cls(**obj)
 
-    Represents an issue with the front side of a document.\n
-    The error is considered resolved when the file with the front side of the document changes.
-    '''
     def __init__(
         self,
-        type: Literal[
-            'passport',
-            'driver_license',
-            'identity_card',
-            'internal_passport'
-        ],
-        file_hash: str,
-        message: str
+        location: Location,
+        title: str,
+        address: str,
+        foursquare_id: Optional[str] = None,
+        foursquare_type: Optional[str] = None,
+        google_place_id: Optional[str] = None,
+        google_place_type: Optional[str] = None
     ):
-        self.source = DEFAULT_PASSPORT_ELEMENT_ERROR_FRONT_SIDE
-        self.type = type
-        self.file_hash = file_hash
-        self.message = message
-
+        self.location = location
+        self.title = title
+        self.address = address
+        self.foursquare_id = foursquare_id
+        self.foursquare_type = foursquare_type
+        self.google_place_id = google_place_id
+        self.google_place_type = google_place_type
 
-class PassportElementErrorReverseSide(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#passportelementerrorreverseside
 
-    Represents an issue with the reverse side of a document.\n
-    The error is considered resolved when the file with reverse side of the document changes.
+class Video(TelegramType):
     '''
-    def __init__(
-        self,
-        type: Literal['driver_license', 'identity_card'],
-        file_hash: str,
-        message: str
-    ):
-        self.source = DEFAULT_PASSPORT_ELEMENT_ERROR_REVERSE_SIDE
-        self.type = type
-        self.file_hash = file_hash
-        self.message = message
+    https://core.telegram.org/bots/api#video
 
+    This object represents a video file.
 
-class PassportElementErrorSelfie(TelegramType):
+    :param file_id: Identifier for this file, which can be used to download or reuse the file.
+    :type file_id: :obj:`str`
+    :param file_unique_id: Unique identifier for this file, which is supposed to be the same over time and for different bots. Can't be used to download or reuse the file.
+    :type file_unique_id: :obj:`str`
+    :param width: Video width as defined by sender.
+    :type width: :obj:`int`
+    :param height: Video height as defined by sender.
+    :type height: :obj:`int`
+    :param duration: Duration of the video in seconds as defined by sender.
+    :type duration: :obj:`int`
+    :param thumbnail: Video thumbnail.
+    :type thumbnail: :obj:`~aiotgm.types.PhotoSize`, optional
+    :param file_name: Original filename as defined by sender.
+    :type file_name: :obj:`str`, optional
+    :param mime_type: MIME type of the file as defined by sender.
+    :type mime_type: :obj:`str`, optional
+    :param file_size: File size in bytes. It can be bigger than 2^31 and some programming languages may have difficulty/silent defects in interpreting it. But it has at most 52 significant bits, so a signed 64-bit integer or double-precision float type are safe for storing this value.
+    :type file_size: :obj:`int`, optional
     '''
-    https://core.telegram.org/bots/api#passportelementerrorselfie
+    @classmethod
+    @_parse_result
+    def _dese(cls, res: dict):
+        obj = {}
+        obj['file_id'] = res.get('file_id')
+        obj['file_unique_id'] = res.get('file_unique_id')
+        obj['width'] = res.get('width')
+        obj['height'] = res.get('height')
+        obj['duration'] = res.get('duration')
+        obj['thumbnail'] = PhotoSize._dese(res.get('thumbnail'))
+        obj['file_name'] = res.get('file_name')
+        obj['mime_type'] = res.get('mime_type')
+        obj['file_size'] = res.get('file_size')
+        return cls(**obj)
 
-    Represents an issue with the selfie with a document.\n
-    The error is considered resolved when the file with the selfie changes.
-    '''
     def __init__(
         self,
-        type: Literal[
-            'passport',
-            'driver_license',
-            'identity_card',
-            'internal_passport'
-        ],
-        file_hash: str,
-        message: str
+        file_id: str,
+        file_unique_id: str,
+        width: int,
+        height: int,
+        duration: int,
+        thumbnail: Optional[PhotoSize] = None,
+        file_name: Optional[str] = None,
+        mime_type: Optional[str] = None,
+        file_size: Optional[int] = None
     ):
-        self.source = DEFAULT_PASSPORT_ELEMENT_ERROR_SELFIE
-        self.type = type
-        self.file_hash = file_hash
-        self.message = message
-
+        self.file_id = file_id
+        self.file_unique_id = file_unique_id
+        self.width = width
+        self.height = height
+        self.duration = duration
+        self.thumbnail = thumbnail
+        self.file_name = file_name
+        self.mime_type = mime_type
+        self.file_size = file_size
 
-class PassportElementErrorFile(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#passportelementerrorfile
 
-    Represents an issue with a document scan.\n
-    The error is considered resolved when the file with the document scan changes.
+class VideoChatEnded(TelegramType):
     '''
-    def __init__(
-        self,
-        type: Literal[
-            'utility_bill',
-            'bank_statement',
-            'rental_agreement',
-            'passport_registration',
-            'temporary_registration'
-        ],
-        file_hash: str,
-        message: str
-    ):
-        self.source = DEFAULT_PASSPORT_ELEMENT_ERROR_FILE
-        self.type = type
-        self.file_hash = file_hash
-        self.message = message
+    https://core.telegram.org/bots/api#videochatended
 
+    This object represents a service message about a video chat ended in the chat.
 
-class PassportElementErrorFiles(TelegramType):
+    :param duration: Video chat duration in seconds.
+    :type duration: :obj:`int`
     '''
-    https://core.telegram.org/bots/api#passportelementerrorfiles
+    @classmethod
+    @_parse_result
+    def _dese(cls, res: dict):
+        obj = {}
+        obj['duration'] = res.get('duration')
+        return cls(**obj)
 
-    Represents an issue with a list of scans.\n
-    The error is considered resolved when the list of files containing the scans changes.
-    '''
     def __init__(
         self,
-        type: Literal[
-            'utility_bill',
-            'bank_statement',
-            'rental_agreement',
-            'passport_registration',
-            'temporary_registration'
-        ],
-        file_hashes: list[str],
-        message: str
+        duration: int
     ):
-        self.source = DEFAULT_PASSPORT_ELEMENT_ERROR_FILES
-        self.type = type
-        self.file_hashes = file_hashes
-        self.message = message
-
+        self.duration = duration
 
-class PassportElementErrorTranslationFile(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#passportelementerrortranslationfile
 
-    Represents an issue with one of the files that constitute the translation of a document.\n
-    The error is considered resolved when the file changes.
+class VideoChatParticipantsInvited(TelegramType):
     '''
-    def __init__(
-        self,
-        type: Literal[
-            'passport',
-            'driver_license',
-            'identity_card',
-            'internal_passport',
-            'utility_bill',
-            'bank_statement',
-            'rental_agreement',
-            'passport_registration',
-            'temporary_registration'
-        ],
-        file_hash: str,
-        message: str
-    ):
-        self.source = DEFAULT_PASSPORT_ELEMENT_ERROR_TRANSLATION_FILE
-        self.type = type
-        self.file_hash = file_hash
-        self.message = message
+    https://core.telegram.org/bots/api#videochatparticipantsinvited
 
+    This object represents a service message about new members invited to a video chat.
 
-class PassportElementErrorTranslationFiles(TelegramType):
+    :param users: New members that were invited to the video chat.
+    :type users: :obj:`list` of :obj:`~aiotgm.types.User`
     '''
-    https://core.telegram.org/bots/api#passportelementerrortranslationfiles
+    @classmethod
+    @_parse_result
+    def _dese(cls, res: dict):
+        obj = {}
+        obj['users'] = [User._dese(kwargs) for kwargs in res.get('users')]
+        return cls(**obj)
 
-    Represents an issue with the translated version of a document.\n
-    The error is considered resolved when a file with the document translation change.
-    '''
     def __init__(
         self,
-        type: Literal[
-            'passport',
-            'driver_license',
-            'identity_card',
-            'internal_passport',
-            'utility_bill',
-            'bank_statement',
-            'rental_agreement',
-            'passport_registration',
-            'temporary_registration'
-        ],
-        file_hashes: list[str],
-        message: str
+        users: list[User]
     ):
-        self.source = DEFAULT_PASSPORT_ELEMENT_ERROR_TRANSLATION_FILES
-        self.type = type
-        self.file_hashes = file_hashes
-        self.message = message
+        self.users = users
 
 
-class PassportElementErrorUnspecified(TelegramType):
+class VideoChatScheduled(TelegramType):
     '''
-    https://core.telegram.org/bots/api#passportelementerrorunspecified
+    https://core.telegram.org/bots/api#videochatscheduled
 
-    Represents an issue in an unspecified place.\n
-    The error is considered resolved when new data is added.
+    This object represents a service message about a video chat scheduled in the chat.
+
+    :param start_date: Point in time (Unix timestamp) when the video chat is supposed to be started by a chat administrator.
+    :type start_date: :obj:`int`
     '''
+    @classmethod
+    @_parse_result
+    def _dese(cls, res: dict):
+        obj = {}
+        obj['start_date'] = res.get('start_date')
+        return cls(**obj)
+
     def __init__(
         self,
-        type: str,
-        element_hash: str,
-        message: str
+        start_date: int
     ):
-        self.source = DEFAULT_PASSPORT_ELEMENT_ERROR_UNSPECIFIED
-        self.type = type
-        self.element_hash = element_hash
-        self.message = message
-
-
-PassportElementError = Union[
-    PassportElementErrorDataField,
-    PassportElementErrorFrontSide,
-    PassportElementErrorReverseSide,
-    PassportElementErrorSelfie,
-    PassportElementErrorFile,
-    PassportElementErrorFiles,
-    PassportElementErrorTranslationFile,
-    PassportElementErrorTranslationFiles,
-    PassportElementErrorUnspecified
-]
-'''
-https://core.telegram.org/bots/api#passportelementerror
-
-This object represents an error in the Telegram Passport element which
-was submitted that should be resolved by the user.
-
-It should be one of:
-
-- PassportElementErrorDataField
-- PassportElementErrorFrontSide
-- PassportElementErrorReverseSide
-- PassportElementErrorSelfie
-- PassportElementErrorFile
-- PassportElementErrorFiles
-- PassportElementErrorTranslationFile
-- PassportElementErrorTranslationFiles
-- PassportElementErrorUnspecified
-'''
-
-# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
+        self.start_date = start_date
 
-# MessageOrigin: 4 SUBCLASSES ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-class MessageOriginUser(TelegramType):
+class VideoChatStarted(TelegramType):
     '''
-    https://core.telegram.org/bots/api#messageoriginuser
+    https://core.telegram.org/bots/api#videochatstarted
 
-    The message was originally sent by a known user.
+    This object represents a service message about a video
+    chat started in the chat. Currently holds no information.
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['date'] = res.get('date')
-        obj['sender_user'] = User._dese(res.get('sender_user'))
         return cls(**obj)
 
-    def __init__(
-        self,
-        date: int,
-        sender_user: User
-    ):
-        self.type = DEFAULT_MESSAGE_ORIGIN_USER
-        self.date = date
-        self.sender_user = sender_user
+    def __init__(self):
+        ...
 
 
-class MessageOriginHiddenUser(TelegramType):
+class VideoNote(TelegramType):
     '''
-    https://core.telegram.org/bots/api#messageoriginhiddenuser
+    https://core.telegram.org/bots/api#videonote
 
-    The message was originally sent by an unknown user.
+    This object represents a `video message <https://telegram.org/blog/video-messages-and-telescope>`_
+    (available in Telegram apps as of `v.4.0 <https://telegram.org/blog/video-messages-and-telescope>`_).
+
+    :param file_id: Identifier for this file, which can be used to download or reuse the file.
+    :type file_id: :obj:`str`
+    :param file_unique_id: Unique identifier for this file, which is supposed to be the same over time and for different bots. Can't be used to download or reuse the file.
+    :type file_unique_id: :obj:`str`
+    :param length: Video width and height (diameter of the video message) as defined by sender.
+    :type length: :obj:`int`
+    :param duration: Duration of the video in seconds as defined by sender.
+    :type duration: :obj:`int`
+    :param thumbnail: Video thumbnail.
+    :type thumbnail: :obj:`~aiotgm.types.PhotoSize`, optional
+    :param file_size: File size in bytes.
+    :type file_size: :obj:`int`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['date'] = res.get('date')
-        obj['sender_user_name'] = res.get('sender_user_name')
+        obj['file_id'] = res.get('file_id')
+        obj['file_unique_id'] = res.get('file_unique_id')
+        obj['length'] = res.get('length')
+        obj['duration'] = res.get('duration')
+        obj['thumbnail'] = PhotoSize._dese(res.get('thumbnail'))
+        obj['file_size'] = res.get('file_size')
         return cls(**obj)
 
     def __init__(
         self,
-        date: int,
-        sender_user_name: str
+        file_id: str,
+        file_unique_id: str,
+        length: int,
+        duration: int,
+        thumbnail: Optional[PhotoSize] = None,
+        file_size: Optional[int] = None
     ):
-        self.type = DEFAULT_MESSAGE_ORIGIN_HIDDEN_USER
-        self.date = date
-        self.sender_user_name = sender_user_name
+        self.file_id = file_id
+        self.file_unique_id = file_unique_id
+        self.length = length
+        self.duration = duration
+        self.thumbnail = thumbnail
+        self.file_size = file_size
 
 
-class MessageOriginChat(TelegramType):
+class Voice(TelegramType):
     '''
-    https://core.telegram.org/bots/api#messageoriginchat
+    https://core.telegram.org/bots/api#voice
 
-    The message was originally sent on behalf of a chat to a group chat.
+    This object represents a voice note.
+
+    :param file_id: Identifier for this file, which can be used to download or reuse the file.
+    :type file_id: :obj:`str`
+    :param file_unique_id: Unique identifier for this file, which is supposed to be the same over time and for different bots. Can't be used to download or reuse the file.
+    :type file_unique_id: :obj:`str`
+    :param duration: Duration of the audio in seconds as defined by sender.
+    :type duration: :obj:`int`
+    :param mime_type: MIME type of the file as defined by sender.
+    :type mime_type: :obj:`str`, optional
+    :param file_size: File size in bytes. It can be bigger than 2^31 and some programming languages may have difficulty/silent defects in interpreting it. But it has at most 52 significant bits, so a signed 64-bit integer or double-precision float type are safe for storing this value.
+    :type file_size: :obj:`int`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['date'] = res.get('date')
-        obj['sender_chat'] = Chat._dese(res.get('sender_chat'))
-        obj['author_signature'] = res.get('author_signature')
+        obj['file_id'] = res.get('file_id')
+        obj['file_unique_id'] = res.get('file_unique_id')
+        obj['duration'] = res.get('duration')
+        obj['mime_type'] = res.get('mime_type')
+        obj['file_size'] = res.get('file_size')
         return cls(**obj)
 
     def __init__(
         self,
-        date: int,
-        sender_chat: Chat,
-        author_signature: Optional[str] = None
+        file_id: str,
+        file_unique_id: str,
+        duration: int,
+        mime_type: Optional[str] = None,
+        file_size: Optional[int] = None
     ):
-        self.type = DEFAULT_MESSAGE_ORIGIN_CHAT
-        self.date = date
-        self.sender_chat = sender_chat
-        self.author_signature = author_signature
+        self.file_id = file_id
+        self.file_unique_id = file_unique_id
+        self.duration = duration
+        self.mime_type = mime_type
+        self.file_size = file_size
 
 
-class MessageOriginChannel(TelegramType):
+class WebAppData(TelegramType):
     '''
-    https://core.telegram.org/bots/api#messageoriginchannel
+    https://core.telegram.org/bots/api#webappdata
 
-    The message was originally sent to a channel chat.
+    Describes data sent from a `Web App <https://core.telegram.org/bots/webapps>`_ to the bot.
+
+    :param data: The data. Be aware that a bad client can send arbitrary data in this field.
+    :type data: :obj:`str`
+    :param button_text: Text of the *web_app* keyboard button from which the Web App was opened. Be aware that a bad client can send arbitrary data in this field.
+    :type button_text: :obj:`str`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['date'] = res.get('date')
-        obj['chat'] = Chat._dese(res.get('chat'))
-        obj['message_id'] = res.get('message_id')
-        obj['author_signature'] = res.get('author_signature')
+        obj['data'] = res.get('data')
+        obj['button_text'] = res.get('button_text')
         return cls(**obj)
 
     def __init__(
         self,
-        date: int,
-        chat: Chat,
-        message_id: int,
-        author_signature: Optional[str] = None
+        data: str,
+        button_text: str
     ):
-        self.type = DEFAULT_MESSAGE_ORIGIN_CHANNEL
-        self.date = date
-        self.chat = chat
-        self.message_id = message_id
-        self.author_signature = author_signature
-
-
-MessageOrigin = Union[
-    MessageOriginUser,
-    MessageOriginHiddenUser,
-    MessageOriginChat,
-    MessageOriginChannel
-]
-'''
-https://core.telegram.org/bots/api#messageorigin
-
-This object describes the origin of a message.
-
-It can be one of:
+        self.data = data
+        self.button_text = button_text
 
-- MessageOriginUser
-- MessageOriginHiddenUser
-- MessageOriginChat
-- MessageOriginChannel
-'''
 
-def _dese_message_origin(res: Optional[dict], /) -> Optional[MessageOrigin]:
-    '''
-    Function to deserialize MessageOrigin.
+class WebAppInfo(TelegramType):
     '''
-    if res is None: return None
-    obj = _check_dict(res)
-
-    type = obj.pop('type')
-
-    if type == DEFAULT_MESSAGE_ORIGIN_USER:
-        return MessageOriginUser._dese(obj, check_dict=False)
-
-    elif type == DEFAULT_MESSAGE_ORIGIN_HIDDEN_USER:
-        return MessageOriginHiddenUser._dese(obj, check_dict=False)
-
-    elif type == DEFAULT_MESSAGE_ORIGIN_CHAT:
-        return MessageOriginChat._dese(obj, check_dict=False)
-
-    elif type == DEFAULT_MESSAGE_ORIGIN_CHANNEL:
-        return MessageOriginChannel._dese(obj, check_dict=False)
-    else:
-        raise ValueError(
-            'An error occurred during the deserialization'
-            f' of the type MessageOrigin. Invalid type: {type!r}.'
-        )
-
-# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
+    https://core.telegram.org/bots/api#webappinfo
 
-class UserChatBoosts(TelegramType):
-    '''
-    https://core.telegram.org/bots/api#userchatboosts
+    Describes a `Web App <https://core.telegram.org/bots/webapps>`_.
 
-    This object represents a list of boosts added to a chat by a user.
+    :param url: An HTTPS URL of a Web App to be opened with additional data as specified in `Initializing Web Apps <https://core.telegram.org/bots/webapps#initializing-mini-apps>`_.
+    :type url: :obj:`str`
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['boosts'] = [ChatBoost._dese(kwargs) for kwargs in res.get('boosts')]
+        obj['url'] = res.get('url')
         return cls(**obj)
 
     def __init__(
         self,
-        boosts: list[ChatBoost]
+        url: str
     ):
-        self.boosts = boosts
+        self.url = url
 
 
-class Update(TelegramType):
+class WriteAccessAllowed(TelegramType):
     '''
-    https://core.telegram.org/bots/api#update
+    https://core.telegram.org/bots/api#writeaccessallowed
+
+    This object represents a service message about a user allowing a bot to write
+    messages after adding it to the attachment menu, launching a Web App from a link,
+    or accepting an explicit request from a Web App sent by the method `requestWriteAccess <https://core.telegram.org/bots/webapps#initializing-mini-apps>`_.
 
-    This object represents an incoming update.\n
-    At most one of the optional parameters can be present in any given update.
+    :param from_request: :obj:`True`, if the access was granted after the user accepted an explicit request from a Web App sent by the method `requestWriteAccess <https://core.telegram.org/bots/webapps#initializing-mini-apps>`_.
+    :type from_request: :obj:`bool`, optional
+    :param web_app_name: Name of the Web App, if the access was granted when the Web App was launched from a link.
+    :type web_app_name: :obj:`str`, optional
+    :param from_attachment_menu: :obj:`True`, if the access was granted when the bot was added to the attachment or side menu.
+    :type from_attachment_menu: :obj:`bool`, optional
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
-        obj['update_id'] = res.get('update_id')
-        obj['message'] = Message._dese(res.get('message'))
-        obj['edited_message'] = Message._dese(res.get('edited_message'))
-        obj['channel_post'] = Message._dese(res.get('channel_post'))
-        obj['edited_channel_post'] = Message._dese(res.get('edited_channel_post'))
-        obj['business_connection'] = BusinessConnection._dese(res.get('business_connection'))
-        obj['business_message'] = Message._dese(res.get('business_message'))
-        obj['edited_business_message'] = Message._dese(res.get('edited_business_message'))
-        obj['deleted_business_messages'] = BusinessMessagesDeleted._dese(res.get('deleted_business_messages'))
-        obj['message_reaction'] = MessageReactionUpdated._dese(res.get('message_reaction'))
-        obj['message_reaction_count'] = MessageReactionCountUpdated._dese(res.get('message_reaction_count'))
-        obj['inline_query'] = InlineQuery._dese(res.get('inline_query'))
-        obj['chosen_inline_result'] = ChosenInlineResult._dese(res.get('chosen_inline_result'))
-        obj['callback_query'] = CallbackQuery._dese(res.get('callback_query'))
-        obj['shipping_query'] = ShippingQuery._dese(res.get('shipping_query'))
-        obj['pre_checkout_query'] = PreCheckoutQuery._dese(res.get('pre_checkout_query'))
-        obj['poll'] = Poll._dese(res.get('poll'))
-        obj['poll_answer'] = PollAnswer._dese(res.get('poll_answer'))
-        obj['my_chat_member'] = ChatMemberUpdated._dese(res.get('my_chat_member'))
-        obj['chat_member'] = ChatMemberUpdated._dese(res.get('chat_member'))
-        obj['chat_join_request'] = ChatJoinRequest._dese(res.get('chat_join_request'))
-        obj['chat_boost'] = ChatBoostUpdated._dese(res.get('chat_boost'))
-        obj['removed_chat_boost'] = ChatBoostRemoved._dese(res.get('removed_chat_boost'))
+        obj['from_request'] = res.get('from_request')
+        obj['web_app_name'] = res.get('web_app_name')
+        obj['from_attachment_menu'] = res.get('from_attachment_menu')
         return cls(**obj)
 
     def __init__(
         self,
-        update_id: int,
-        message: Optional[Message] = None,
-        edited_message: Optional[Message] = None,
-        channel_post: Optional[Message] = None,
-        edited_channel_post: Optional[Message] = None,
-        business_connection: Optional[BusinessConnection] = None,
-        business_message: Optional[Message] = None,
-        edited_business_message: Optional[Message] = None,
-        deleted_business_messages: Optional[BusinessMessagesDeleted] = None,
-        message_reaction: Optional[MessageReactionUpdated] = None,
-        message_reaction_count: Optional[MessageReactionCountUpdated] = None,
-        inline_query: Optional[InlineQuery] = None,
-        chosen_inline_result: Optional[ChosenInlineResult] = None,
-        callback_query: Optional[CallbackQuery] = None,
-        shipping_query: Optional[ShippingQuery] = None,
-        pre_checkout_query: Optional[PreCheckoutQuery] = None,
-        poll: Optional[Poll] = None,
-        poll_answer: Optional[PollAnswer] = None,
-        my_chat_member: Optional[ChatMemberUpdated] = None,
-        chat_member: Optional[ChatMemberUpdated] = None,
-        chat_join_request: Optional[ChatJoinRequest] = None,
-        chat_boost: Optional[ChatBoostUpdated] = None,
-        removed_chat_boost: Optional[ChatBoostRemoved] = None
+        from_request: Optional[bool] = None,
+        web_app_name: Optional[str] = None,
+        from_attachment_menu: Optional[bool] = None
     ):
-        self.update_id = update_id
-        self.message = message
-        self.edited_message = edited_message
-        self.channel_post = channel_post
-        self.edited_channel_post = edited_channel_post
-        self.business_connection = business_connection
-        self.business_message = business_message
-        self.edited_business_message = edited_business_message
-        self.deleted_business_messages = deleted_business_messages
-        self.message_reaction = message_reaction
-        self.message_reaction_count = message_reaction_count
-        self.inline_query = inline_query
-        self.chosen_inline_result = chosen_inline_result
-        self.callback_query = callback_query
-        self.shipping_query = shipping_query
-        self.pre_checkout_query = pre_checkout_query
-        self.poll = poll
-        self.poll_answer = poll_answer
-        self.my_chat_member = my_chat_member
-        self.chat_member = chat_member
-        self.chat_join_request = chat_join_request
-        self.chat_boost = chat_boost
-        self.removed_chat_boost = removed_chat_boost
+        self.from_request = from_request
+        self.web_app_name = web_app_name
+        self.from_attachment_menu = from_attachment_menu
+
+
+#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+REPLY_MARKUP_TYPES = Union[InlineKeyboardMarkup, ReplyKeyboardMarkup, ReplyKeyboardRemove, ForceReply]
+'''
+One of the following reply markups:
+
+- :obj:`~aiotgm.types.InlineKeyboardMarkup`
+- :obj:`~aiotgm.types.ReplyKeyboardMarkup`
+- :obj:`~aiotgm.types.ReplyKeyboardRemove`
+- :obj:`~aiotgm.types.ForceReply`
+'''
 
 
 BotCommandScope = Union[
     BotCommandScopeDefault,
     BotCommandScopeAllPrivateChats,
     BotCommandScopeAllGroupChats,
     BotCommandScopeAllChatAdministrators,
@@ -7679,7 +8348,171 @@
 - :obj:`~aiotgm.types.InputLocationMessageContent`
 - :obj:`~aiotgm.types.InputVenueMessageContent`
 - :obj:`~aiotgm.types.InputContactMessageContent`
 - :obj:`~aiotgm.types.InputInvoiceMessageContent`
 '''
 
 
+MaybeInaccessibleMessage = Union[Message, InaccessibleMessage]
+'''
+https://core.telegram.org/bots/api#maybeinaccessiblemessage
+
+This object describes a message that can be inaccessible to the bot. It can be one of:
+
+- :obj:`~aiotgm.types.Message`
+- :obj:`~aiotgm.types.InaccessibleMessage`
+'''
+
+def _dese_maybe_inaccessible_message(res: Optional[dict], /) -> Optional[MaybeInaccessibleMessage]:
+    '''
+    Function to deserialize MaybeInaccessibleMessage.
+    '''
+    if res is None: return None
+    obj = _check_dict(res)
+
+    if obj['date'] == 0:
+        return InaccessibleMessage._dese(obj, check_dict=False)
+    else:
+        return Message._dese(obj, check_dict=False)
+
+
+MenuButton = Union[MenuButtonCommands, MenuButtonWebApp, MenuButtonDefault]
+'''
+https://core.telegram.org/bots/api#menubutton
+
+This object describes the bot's menu button in a private chat. It should be one of
+
+- :obj:`~aiotgm.types.MenuButtonCommands`
+- :obj:`~aiotgm.types.MenuButtonWebApp`
+- :obj:`~aiotgm.types.MenuButtonDefault`
+
+If a menu button other than :obj:`~aiotgm.types.MenuButtonDefault` is set for a private
+chat, then it is applied in the chat. Otherwise the default menu button is applied. By
+default, the menu button opens the list of bot commands.
+'''
+
+def _dese_menu_button(res: Optional[dict], /) -> Optional[MenuButton]: # used in aiotgm.__init__
+    '''
+    Function to deserialize MenuButton.
+    '''
+    if res is None: return None
+    obj = _check_dict(res)
+
+    type = obj.pop('type')
+
+    if type == DEFAULT_MENU_BUTTON_COMMANDS:
+        return MenuButtonCommands._dese(obj, check_dict=False)
+
+    elif type == DEFAULT_MENU_BUTTON_WEB_APP:
+        return MenuButtonWebApp._dese(obj, check_dict=False)
+
+    elif type == DEFAULT_MENU_BUTTON_DEFAULT:
+        return MenuButtonDefault._dese(obj, check_dict=False)
+    else:
+        raise ValueError(
+            'An error occurred during the deserialization'
+            f' of the type MenuButton. Invalid type: {type!r}.'
+        )
+
+
+MessageOrigin = Union[
+    MessageOriginUser,
+    MessageOriginHiddenUser,
+    MessageOriginChat,
+    MessageOriginChannel
+]
+'''
+https://core.telegram.org/bots/api#messageorigin
+
+This object describes the origin of a message. It can be one of:
+
+- :obj:`~aiotgm.types.MessageOriginUser`
+- :obj:`~aiotgm.types.MessageOriginHiddenUser`
+- :obj:`~aiotgm.types.MessageOriginChat`
+- :obj:`~aiotgm.types.MessageOriginChannel`
+'''
+
+def _dese_message_origin(res: Optional[dict], /) -> Optional[MessageOrigin]:
+    '''
+    Function to deserialize MessageOrigin.
+    '''
+    if res is None: return None
+    obj = _check_dict(res)
+
+    type = obj.pop('type')
+
+    if type == DEFAULT_MESSAGE_ORIGIN_USER:
+        return MessageOriginUser._dese(obj, check_dict=False)
+
+    elif type == DEFAULT_MESSAGE_ORIGIN_HIDDEN_USER:
+        return MessageOriginHiddenUser._dese(obj, check_dict=False)
+
+    elif type == DEFAULT_MESSAGE_ORIGIN_CHAT:
+        return MessageOriginChat._dese(obj, check_dict=False)
+
+    elif type == DEFAULT_MESSAGE_ORIGIN_CHANNEL:
+        return MessageOriginChannel._dese(obj, check_dict=False)
+    else:
+        raise ValueError(
+            'An error occurred during the deserialization'
+            f' of the type MessageOrigin. Invalid type: {type!r}.'
+        )
+
+
+PassportElementError = Union[
+    PassportElementErrorDataField,
+    PassportElementErrorFrontSide,
+    PassportElementErrorReverseSide,
+    PassportElementErrorSelfie,
+    PassportElementErrorFile,
+    PassportElementErrorFiles,
+    PassportElementErrorTranslationFile,
+    PassportElementErrorTranslationFiles,
+    PassportElementErrorUnspecified
+]
+'''
+https://core.telegram.org/bots/api#passportelementerror
+
+This object represents an error in the Telegram Passport element which
+was submitted that should be resolved by the user. It should be one of:
+
+- :obj:`~aiotgm.types.PassportElementErrorDataField`
+- :obj:`~aiotgm.types.PassportElementErrorFrontSide`
+- :obj:`~aiotgm.types.PassportElementErrorReverseSide`
+- :obj:`~aiotgm.types.PassportElementErrorSelfie`
+- :obj:`~aiotgm.types.PassportElementErrorFile`
+- :obj:`~aiotgm.types.PassportElementErrorFiles`
+- :obj:`~aiotgm.types.PassportElementErrorTranslationFile`
+- :obj:`~aiotgm.types.PassportElementErrorTranslationFiles`
+- :obj:`~aiotgm.types.PassportElementErrorUnspecified`
+'''
+
+
+ReactionType = Union[ReactionTypeEmoji, ReactionTypeCustomEmoji]
+'''
+https://core.telegram.org/bots/api#reactiontype
+
+This object describes the type of a reaction. Currently, it can be one of:
+
+- :obj:`~aiotgm.types.ReactionTypeEmoji`
+- :obj:`~aiotgm.types.ReactionTypeCustomEmoji`
+'''
+
+def _dese_reaction_type(res: Optional[dict], /) -> Optional[ReactionType]:
+    '''
+    Function to deserialize ReactionType.
+    '''
+    if res is None: return None
+    obj = _check_dict(res)
+
+    type = obj.pop('type')
+
+    if type == DEFAULT_REACTION_TYPE_EMOJI:
+        return ReactionTypeEmoji._dese(obj, check_dict=False)
+
+    elif type == DEFAULT_REACTION_TYPE_CUSTOM_EMOJI:
+        return ReactionTypeCustomEmoji._dese(obj, check_dict=False)
+    else:
+        raise ValueError(
+            'An error occurred during the deserialization'
+            f' of the type ReactionType. Invalid type: {type!r}.'
+        )
```

### Comparing `aiotgm-0.3.5/aiotgm/update_manager.py` & `aiotgm-0.3.6/aiotgm/update_manager.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.5/aiotgm/utils.py` & `aiotgm-0.3.6/aiotgm/utils.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.5/aiotgm.egg-info/PKG-INFO` & `aiotgm-0.3.6/aiotgm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotgm
-Version: 0.3.5
+Version: 0.3.6
 Author: unixtux
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `aiotgm-0.3.5/tests/test_func_ok.py` & `aiotgm-0.3.6/tests/test_func_ok.py`

 * *Files identical despite different names*

