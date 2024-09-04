-- Representación en CHAR para letras con acento y caracteres especiales en SQL Server

-- Letras minúsculas con acento:
-- á → CHAR(225)
-- é → CHAR(233)
-- í → CHAR(237)
-- ó → CHAR(243)
-- ú → CHAR(250)
-- ñ → CHAR(241)

-- Letras mayúsculas con acento:
-- Á → CHAR(193)
-- É → CHAR(201)
-- Í → CHAR(205)
-- Ó → CHAR(211)
-- Ú → CHAR(218)
-- Ñ → CHAR(209)

-- Caracteres especiales:
-- @ → CHAR(64)
-- / → CHAR(47)
-- \ → CHAR(92)
-- # → CHAR(35)

SELECT 
    CHAR(225) AS 'á', 
    CHAR(233) AS 'é', 
    CHAR(237) AS 'í', 
    CHAR(243) AS 'ó', 
    CHAR(250) AS 'ú', 
    CHAR(241) AS 'ñ',
    CHAR(193) AS 'Á',
    CHAR(201) AS 'É',
    CHAR(205) AS 'Í',
    CHAR(211) AS 'Ó',
    CHAR(218) AS 'Ú',
    CHAR(209) AS 'Ñ',
    CHAR(64)  AS '@',
    CHAR(47)  AS '/',
    CHAR(92)  AS '\',
    CHAR(35)  AS '#';
