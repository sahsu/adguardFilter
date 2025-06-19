# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a personal AdGuard filter repository containing custom ad-blocking rules. The main filter file is consumed by AdGuard applications via the GitHub raw URL: `https://raw.githubusercontent.com/sahsu/adguardFilter/master/filter.txt`

## Key Files

- `filter.txt` - Main AdGuard filter file containing blocking rules (~1200 lines)
- `README.md` - Basic usage instructions

## Filter Rule Format

The filter.txt file uses AdGuard filter syntax:
- Lines starting with `!` are comments with dates and URLs
- `##` selectors hide elements (cosmetic filtering)
- `||` rules block domains/URLs
- Rules are organized chronologically by when they were added

## Development Workflow

When modifying filters:
1. Add new blocking rules to `filter.txt`
2. Include comment with date and target URL above new rules
3. Test rules in AdGuard before committing
4. Commit with descriptive message (usually "update" + description)

## Git Usage

- Main branch: `main`
- Current development happens on feature branches
- Commit messages are typically simple: "update", "add [site]", "update for [site]"