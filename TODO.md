Implement

  CPU (6502)
    Registers
      A register (Accumulator)
      X register
      Y register
      Status register
    Stack Pointer
    Program Counter
    
    Debugger for instructions
      Space key for next instruction
    
  PPU
  
  First GUI in console
  Later develop a proper display emulator

Test CPU functionaliy by doing a 3 * 10 multiplication:

*=$8000
			LDX #10
			STX $0000
			LDX #3
			STX $0001
			LDY $0000
			LDA #0
			CLC
			loop
			ADC $0001
			DEY
			BNE loop
			STA $0002
			NOP
			NOP
			NOP
