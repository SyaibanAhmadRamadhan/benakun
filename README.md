
# BenAkun Free Accounting Software

free double-entry bookeeping accounting software for Indonesian personal or soho business (UMKM).

based on:
- http://iaiglobal.or.id/v03/files/draft_ed_sak_emkm_kompilasi.pdf
- http://iaiglobal.or.id/v03/files/file_sak/emkm/
- https://www.youtube.com/watch?v=DojvxP_rbH0
- https://www.youtube.com/watch?v=kP_dHnRC3yk

## Draft Specification

https://docs.google.com/document/d/11u00Ch0oE0EEIGylYg4FlDKLoTWySnHonpFznSPb5Ik/edit?usp=sharing

## Roles

- SuperAdmin
  - can manage tenants
  - can manage users
  - can manage standard CoA (Chart of Account that all company must have)
  - can create entry-rule template
- TenantAdmin
  - can edit company
  - can manage account source
	- can manage users
	- can manage accounts
	- can manage journals
	- can manage reports
  - can manage CoA
  - can manage entry-rule
  - can manage bank account
  - can manage external company (customer, supplier, etc)
  - can manage service/product/stock
  - can backup/restore database
- EntryUser
  - can input transaction/entry and proof
  - can request for update/delete entry and proof
- Guest
  - can register as new tenant
  - can join invitation link to a company
  - can forgot/request reset password
  - can reset password
  - can login

## Features

- [ ] multi-tenant
- [ ] two language (ID, EN)
- [ ] multi-currency (USD, EUR, IDR)
- [ ] multi-user tenant (one tenant can have many users)
- [ ] Reports / Laporan (TODO: find what are the standards and how to use calculate them)
  - [ ] Profit and Loss / Laporan Laba Rugi --> priority
  - [ ] Balance Sheet / Laporan Posisi/Neracaya Keuangan --> priority
  - [ ] Cash Flow / Laporan Arus Kas
  - [ ] Statement of Changes in Equity / Laporan Perubahan Ekuitas/Modal
  - [ ] Notes to Financial Statements / Catatan atas Laporan Keuangan
  - [ ] Other Comprehensive Income / Laporan Laba Rugi Komprehensif Lain
  - [ ] Statement of Financial Position / Laporan Posisi Keuangan
  - [ ] Statement of Comprehensive Income / Laporan Laba Rugi Komprehensif
  - [ ] Statement of Changes in Equity / Laporan Perubahan Ekuitas
  - [ ] Statement of Cash Flows / Laporan Arus Kas
  - [ ] Notes to Financial Statements / Catatan atas Laporan Keuangan
  - [ ] Other Comprehensive Income / Laporan Laba Rugi Komprehensif Lain
  - [ ] laporan penjualan (TODO: find english term)
  - [ ] pergerakan piutang (TODO: find english term)
  - [ ] pergerakan hutang (TODO: find english term)
- [ ] generate invoice
- [ ] generate receipt
- [ ] upload proof

## Design

- per tenant table
- TODO: database design