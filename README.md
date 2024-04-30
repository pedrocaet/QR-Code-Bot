# QR-Code-Bot
Um bot, hospedado no Telegram, cujo foi é configurado pelo código do Repositório. O bot funciona enquanto o código estiver rodando.
Esse bot foi criado durante uma Oficina que presenciei na universidade.

De início, é necessário saber que o Bot é feito no Telegram, com o auxílio do Bot Father, um bot verificado, que hospeda bots.

Para iniciar, instale no código os requests a seguir:
!pip install requests aiogram qrcode

Além dos imports:

from typing import Any, Dict
import qrcode
from aiogram import Bot, Dispatcher, F, Router
from aiogram.enums import ParseMode
from aiogram.filters import CommandStart
from aiogram.fsm.context import FSMContext
from aiogram.fsm.state import State, StatesGroup
from aiogram.types import BufferedInputFile
from io import BytesIO
from aiogram.types import (
    KeyboardButton,
    Message,
    ReplyKeyboardMarkup,
    ReplyKeyboardRemove,
)

que são necessários para o funcionamento do Bot
