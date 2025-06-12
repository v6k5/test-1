function script.onPlayerConnect(playerId)
    ac.sendChatMessage("Welcome to A-Way Team")
    ac.sendChatMessage("Discord server: https://discord.gg/9-3")
end

function script.onChatMessage(playerId, message)
    if message == "/tp" or message == "/legal" or message == "/help" then
        ac.sendChatMessage("أوامر غير مفعلة حالياً، تواصل معنا عبر الديسكورد.")
        return true -- يمنع ظهور رسالة الخطأ الافتراضية
    end
end
