# base666q
Detecting Identical Transaction Payloads
payloads = [tx.input for tx in block.transactions]
if len(payloads) != len(set(payloads)):
    print("Duplicate calldata detected")
