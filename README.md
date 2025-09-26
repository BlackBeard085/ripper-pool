# How to Deposit and Withdraw into Ripper Pool

This guide walks you through cloning the repository, building the program, and performing deposit and withdrawal transactions in Ripper Pool.

---

## Prerequisites

- [Rust](https://www.rust-lang.org/tools/install) installed
- [Cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html) (comes with Rust)
- Access to a Solana wallet with sufficient funds

---

## Step 1: Clone the Repository

Open your terminal and run:

```bash
git clone https://github.com/BlackBeard085/ripper-pool.git
```

Navigate into the `stake-pool` directory:

```bash
cd ripper-pool/stake-pool
```

---

## Step 2: Build the SPL Stake Pool Program

Compile the program in release mode:

```bash
cargo build --release
```

This will generate the executable in:

```bash
target/release/spl-stake-pool
```

---

## Step 3: Deposit into Ripper Pool

Run the deposit command with your wallet's deposit address and amount:

```bash
~/ripper-pool/stake-pool/target/release/spl-stake-pool deposit-sol R1PP3RkqTJniWgzJgeymd4rFpdpXcmjywVomMpd8eAY <AMOUNT>
```

Replace `<AMOUNT>` with the amount of SOL you want to deposit.

---

## Step 4: Withdraw from Ripper Pool

Run the withdrawal command with your deposit address, withdrawal address, and amount:

```bash
~/ripper-pool/stake-pool/target/release/spl-stake-pool withdraw-sol R1PP3RkqTJniWgzJgeymd4rFpdpXcmjywVomMpd8eAY <WITHDRAW-ADDRESS> <AMOUNT>
```

Replace `<WITHDRAW-ADDRESS>` with the address where you want to receive the funds, and `<AMOUNT>` with the amount to withdraw.

---

## Notes
- Ensure your wallet is connected and has enough SOL for transactions and fees.
- Double-check addresses before executing commands.

---

## Support

For further assistance, refer to the repository or contact the maintainer.

---

*Happy staking with Ripper Pool!*
