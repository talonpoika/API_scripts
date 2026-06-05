# API_scripts

A collection of utility scripts for querying security and infrastructure APIs.

## Scripts

### `search_urlscanio_for_asn.ps1`

Searches [urlscan.io](https://urlscan.io) for all domains associated with a given ASN (Autonomous System Number) and exports unique results to a CSV file.

**Requirements**
- PowerShell
- A valid [urlscan.io API key](https://urlscan.io/user/signup)

**Setup**

Set your API key in the script:
```powershell
$apiKey = "your-api-key-here"
```

**Usage**
```powershell
.\search_urlscanio_for_asn.ps1 -asnNumber AS200593
```

**Output**

Creates `result_urlscanio_<asn>.csv` with one unique domain per row.

## License

[GPL-3.0](LICENSE)
