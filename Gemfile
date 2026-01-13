source "https://rubygems.org"
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby "3.2.9"

# Rails本体
gem "rails", "~> 7.1.0"

# 基本的なgem
gem "sprockets-rails"
gem "puma", ">= 5.0"
gem "importmap-rails"
gem "turbo-rails"
gem "stimulus-rails"
gem "jbuilder"
gem "tzinfo-data", platforms: %i[ windows jruby ]
gem "bootsnap", require: false

# ▼▼▼ ここが重要：開発とテスト環境だけ SQLite3 を使う ▼▼▼
group :development, :test do
  gem "sqlite3"
  gem "debug", platforms: %i[ mri mingw x64_mingw ]
end

# 開発環境用ツール
group :development do
  gem "web-console"
end

# テスト環境用ツール
group :test do
  gem "capybara"
  gem "selenium-webdriver"
end

# ▼▼▼ ここが重要：本番環境（Render）は Postgres を使う ▼▼▼
group :production do
  gem "pg"
end