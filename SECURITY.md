-- Auto Farm für All Star Tower Defense X - Infinite Mode
-- Läuft automatisch: Platziert, upgraded und startet Wellen

local Library = loadstring(game:HttpGet("https://pastebin.com/raw/8Qq1xA3H"))() -- Beispiel Library für Auto Place/Upgrade

local function AutoFarm()
    while true do
        -- Automatisch Türme platzieren (an vorgegebenen Stellen)
        Library.AutoPlace = true

        -- Automatisch Türme upgraden
        Library.AutoUpgrade = true

        -- Automatisch Wellen starten und fortsetzen
        Library.AutoWave = true

        -- Automatisch Replay starten (bei Infinite Mode)
        Library.AutoReplay = true

        wait(1) -- Pause, damit das Script nicht zu schnell läuft
    end
end

coroutine.wrap(AutoFarm)()
