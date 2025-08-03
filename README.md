# Controllo LED con STM32 Nucleo

## Descrizione del progetto

Questo è un progetto semplice sviluppato su una board **STM32 Nucleo**, in cui un **LED esterno** viene acceso o spento premendo un **pulsante** (anch'esso esterno). L'obiettivo è mostrare il funzionamento base dell'I/O digitale su una scheda STM32.

## Funzionamento

- Alla pressione del pulsante, il LED cambia stato (ON/OFF).
- Il comportamento è gestito via codice all'interno di un ciclo principale (`main loop`), con logica semplice e diretta.
- Non sono usate interruzioni: il codice legge lo stato del pulsante a ogni iterazione.

## Collegamenti hardware

- **Pulsante** collegato al pin **D4** (GPIO input)
- **LED** collegato al pin **D5** (GPIO output)
- Resistenze di pull-down/pull-up usate dove necessario

> ⚠️ Nota: i componenti (LED, pulsante, resistenze) sono **esterni alla scheda** Nucleo.

## Toolchain

- **IDE utilizzato**: STM32CubeIDE
- **Microcontrollore**: STM32 NUCLEO L476RG
- **Linguaggio**: C

## Possibili estensioni

- Gestione tramite interrupt
- Debouncing software
- Utilizzo di più LED o pulsanti
- Aggiunta di un feedback via UART o LCD

## Schema

![WhatsApp Image 2025-08-03 at 19 29 55](https://github.com/user-attachments/assets/a993042f-4dc1-42e7-acbd-391db046dbbe)



## Licenza

Progetto realizzato a scopo didattico.
