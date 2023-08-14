from pyrogram import Client, filters, types
from config import prefix
import asyncio

@Client.on_message(filters.command("чел", prefixes=prefix) & filters.me)
async def function_name(client, message):
    await message.edit("чел")
    await asyncio.sleep(2)
    await message.edit("ты")
    await asyncio.sleep(2)
    await message.edit("просто")
    await asyncio.sleep(2)
    await message.edit("клоун")
    await asyncio.sleep(2)
    await message.edit("которы нечего не умеет делать")
