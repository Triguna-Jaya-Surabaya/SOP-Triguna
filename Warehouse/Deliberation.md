# System Stock
  - Invoice keluar and simpo
  - Invoice keluar tambah stock via simpo
  - Pindah gudang
  - 

# Stock Masuk
- Simpo
- Spucinv
  - Cons: Only kadm_sby can do it
  - Pros: Explicit record of stock movement kept by the system


# Teams
- 4 people alternating every 3 days
  - Cons: 1 team always avoiding mondays
- 4 people alternating every 6 days 
  - Cons: Less overall team cohesion
- 4 people alternating every 6 days with wednesday in between
  - Cons: should lessen damang against team cohesion (Need to know how they spend their sundays/ask them) #Investigate


# Dorm
- Dorm 6 people with 3 rooms + a folding bed for temporary stays
- Dorm with 4 people, 2 rooms and holding house for 6 people with 2 half rooms. 
  - Half rooms aren't needed because rent is probably cheap, and they'd quickly move because it's very no amenities
  - Half rooms aren't needed cause I have 6 + 4 beds combined, it has to be enough

# Cabang Setting
- Sidoarjo n Surabaya 1 cabang
- Sidoarjo n Surabaya beberapa cabang
  - Pros: Customer checkout, alamat otomatis sesuai
  - Pros: Customer checkout, stock otomatis sesuai
  - Cons: Ribet admin isi stock in out. 
    (Note: Utk Checkoutin customer seharusnya masih gampang)
  1. Harus ganti tbljne saat pindah Main_Office #Action

# Stock Balancing - Shipping
- Balancing from Smaller_Branch to Main_Branch is easy logistically, can be done on car return
- Balanceing from Main_Branch to Smaller_Branch is harder logistically, needs to be on car departure (takes shipping space)


# Shipping SJ Printing
 - Send cart link
 - Send SJ/invoice immediately
   - Pros: Works at scale / after role reversal [[Current#Week Stable|Week Stable]]
   - Pros: immediate loading after pallet
   - Cons: Harder to teach for Team Sidoarjo due to multiple workflows


# Weeks before starting ops
- 2 Months
- 2 Weeks
	- Cons: Ga bisa test buat rame olshop secara strategis dan pelan2
	- Cons: Harus ada admin olshop untuk maintain, coba ubah2 harga secara cepat supaya rame [[SOP#Admin]]
	- Cons: Ada kemungkinan sepi di bulan pertama
	- Cons: Orang gudang harus bantu packing, Banyak pindah2 bagian gudang dan packing dan picker
		- Fix: Week 4 di mana tambah orang dan bagi peran masing2 (Misal 2 gudang, 4 packing)
	- Pros: Less Idle worker = More Team Cohesion (Less drama)
	- Pros: Stress-test SOP
	- Pros: Bigger Revenue, less wasted rent
	- Pros: Less idle wage spending

# Week2n4
- When should Sidoarjo stocks all SKU?
- When should I meet the suppliers and ask them to directly do my fullfillment?
	- This depends on TGR logistic limit
	- I should meet suppliers once I'm ready. I must meet suppliers once we reach TGR logistic limit or SBY will stall because of not enough stock
	- One extra Fuso a week is not a problem for TGR
		- One Fuso helps SBY because it frees a little more space for other items
		- But the packing space is still limited by a single floor
		- SBY would be great if we had a whole floor for packing and a whole floor for picking
		- But that would require at least 2 supplier from Jawa Timur to directly feed Sidoarjo, other than Oripack and Victory
- What if I don't meet the suppliers and only keep Oripack and Victory
	- Items will need to be balanced from Surabaya to Sidoarjo
		- a. balance some items just to keep it running
		- b. balance all items, taking from Surabaya which is still the Main Warehouse at this point
			- Pros: Sidoarjo might have small sales for months
			- Pros: Shipping can be done primarily from Sidoarjo
			- 
		- c. 
		- ~~c. Role Reverse it immediately? This is weakest so far~~

# Pallet
- Plastic pallets with plywood 
- Plastic pallets with plywood and wooden blocks edges
	- Pros: Needs Construction_Team time anyways because we need to layer plywood on top of the plastic pallets so that it doesn't keep breaking, seriously.
	- Pros: Wider (?)
	- Pros: Taller (?)
	- Cons: takes Construction_Team time
	- ~~Cons: can't be used in SBY if needed~~

# Week4n8
- ~~SBY only gets Stock Balancing no Tronton (Why would I do this?)~~
- SBY still gets Tronton
	- ~~a. SBY gets primary always gets Tronton 1/week whenever stock is < 0.5~~
	- b. Less stock gets primary
		- if SDA has less kali_max_gdg then go to SDA?
		- if SBY has less kali_max_gdg then go to SBY?
	- b. SDA gets primary always gets Tronton 1/week whenever stock is < 0.5

# Main_Office Handover
- Handover to SBY
	- SDA Create the invoice, tell SBY to process the invoice
		- Create Invoice - SDA
		- Handle bukti transfer - SDA
			- Technically possible for SBY to handle it. 
			- Cons: one WA login must be used in SBY
			- Cons: not scalable after multi-warehouse, one WA login must be used in SBY
			- Cons: money responsibility is sent to multiple places
			- Pros: ??? Less load??? Less coordination???
			1. SDA sends Nomor Invoice
			2. SBY opens chat, checks invoice
			3. SBY process invoice (go to 2)
		- Handle process invoice - SBY
			- Pros: SDA only needs to send invoice
			- Cons: SDA "should" be the one to handle stock in stock out
			- nvm, even if SDA process, SBY can still print. what am I thinking 🤦‍♂️
		- Handle print invoice - SBY 


# Main_Office Migration
## SBY 1 Chatting + 1 Printing
- Main Office move to SDA  [[Deliberation#Main_Office 2 Chatting]] reside if 1 person is at each location? 
- SDA
- ~~SBY~~
	- Pros: Nothing changes
	- Pros: Less handover
	- Pros: There's a bunch of Ambil Sendiri transactions that needs to be handled in SBY
	- Cons: There's only 1 person in SBY to handle all of the workload, some needs to be shifted to SDA
	- Cons: Main Office will eventually be moved to SDA. Training people in SBY to move in SDA is... Wasteful.
	- Cons: Less bandwidth for training, bandwidth filled with chat replies.

## SBY 2 Printing (?) 