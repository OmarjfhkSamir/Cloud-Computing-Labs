# Lab 3 — Cloud Issue Tracker Architecture

## 1. Application Goal

## 2. Functional Scope

## 3. Request Flow

## 4. Trust Boundaries

User → Frontend form → POST /api/issues → API validation → Data layer
← Render created issue ← 201 + JSON

Page load → GET /api/issues → API → Data layer
← Render list ← 200 + JSON array ←───┘

Button → PATCH /api/issues/{id}/status → API validation → Data layer

USER-CONTROLLED SIDE APPLICATION-CONTROLLED SIDE
Browser input ───── HTTP request ─────▶ REST API ─────▶ Data
▲ │
└────────── JSON response ◀─────────
