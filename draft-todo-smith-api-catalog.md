---
###
# Internet-Draft Markdown Template
#
# Rename this file from draft-todo-yourname-protocol.md to get started.
# Draft name format is "draft-<yourname>-<workgroup>-<name>.md".
#
# For initial setup, you only need to edit the first block of fields.
# Only "title" needs to be changed; delete "abbrev" if your title is short.
# Any other content can be edited, but be careful not to introduce errors.
# Some fields will be set automatically during setup if they are unchanged.
#
# Don't include "-00" or "-latest" in the filename.
# Labels in the form draft-<yourname>-<workgroup>-<name>-latest are used by
# the tools to refer to the current version; see "docname" for example.
#
# This template uses kramdown-rfc: https://github.com/cabo/kramdown-rfc
# You can replace the entire file if you prefer a different format.
# Change the file extension to match the format (.xml for XML, etc...)
#
###
title: "api-catalog: A well-known URI to help discovery of APIs"
abbrev: "api-catalog"
category: standards

docname: draft-smith-api-catalog
submissiontype: IETF
number:
date:
consensus: true
v: 3
area: AREA
workgroup: httpapis
keyword:
 - API
 - well-known
venue:
  group: WG
  type: Working Group
  mail: WG@example.com
  arch: https://example.com/WG
  github: USER/REPO
  latest: https://example.com/LATEST

author:
 -
    fullname: Kevin Smith
    organization: Vodafone
    email: kevin.smith@vodafone.com

normative:
 RFC9264:
 RFC8615:
 RFC6415:
 RFC8288:
informative:
 RFC2119:

--- abstract

This document defines the "api-catalog" well-known URI. It is intended to facilitate discovery of the APIs published by a Web host.


--- middle

# Introduction

A Web host may publish Application Programming Interfaces (APIs) to encourage requests for interaction from  external parties. Such APIs must be discovered before they may be used - i.e., the external party needs to know what APIs a given Web host exposes, including their purpose, any constraints to use, and the endpoints to interact with the APIs. To faciliate discovery of this information, this document proposes a well-known URI, 'api-catalog', as a location where a Web host's API endpoints are listed and described.


# Goals and non-goals

The primary goal is to facilitate the discovery of both a Web Host's public API endpoints, and metadata that informs the potential API client of the purpose of each API and any constraints around usage.
			
Non-goals: this document does not mandate paths for API endpoints. i.e., it is not mandating that my_example_api should be available at `example.com/.well-known/api-catalog/my_example_api` (although it is not forbidden to do so).


# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
