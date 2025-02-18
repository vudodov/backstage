## API Report File for "@backstage/config"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts
// Warning: (ae-missing-release-tag) "AppConfig" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export type AppConfig = {
  context: string;
  data: JsonObject;
  filteredKeys?: string[];
};

// Warning: (ae-missing-release-tag) "Config" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export type Config = {
  subscribe?(onChange: () => void): {
    unsubscribe: () => void;
  };
  has(key: string): boolean;
  keys(): string[];
  get<T = JsonValue>(key?: string): T;
  getOptional<T = JsonValue>(key?: string): T | undefined;
  getConfig(key: string): Config;
  getOptionalConfig(key: string): Config | undefined;
  getConfigArray(key: string): Config[];
  getOptionalConfigArray(key: string): Config[] | undefined;
  getNumber(key: string): number;
  getOptionalNumber(key: string): number | undefined;
  getBoolean(key: string): boolean;
  getOptionalBoolean(key: string): boolean | undefined;
  getString(key: string): string;
  getOptionalString(key: string): string | undefined;
  getStringArray(key: string): string[];
  getOptionalStringArray(key: string): string[] | undefined;
};

// Warning: (ae-missing-release-tag) "ConfigReader" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export class ConfigReader implements Config {
  constructor(
    data: JsonObject | undefined,
    context?: string,
    fallback?: ConfigReader | undefined,
    prefix?: string,
  );
  // (undocumented)
  static fromConfigs(configs: AppConfig[]): ConfigReader;
  // (undocumented)
  get<T = JsonValue>(key?: string): T;
  // (undocumented)
  getBoolean(key: string): boolean;
  // (undocumented)
  getConfig(key: string): ConfigReader;
  // (undocumented)
  getConfigArray(key: string): ConfigReader[];
  // (undocumented)
  getNumber(key: string): number;
  // (undocumented)
  getOptional<T = JsonValue>(key?: string): T | undefined;
  // (undocumented)
  getOptionalBoolean(key: string): boolean | undefined;
  // (undocumented)
  getOptionalConfig(key: string): ConfigReader | undefined;
  // (undocumented)
  getOptionalConfigArray(key: string): ConfigReader[] | undefined;
  // (undocumented)
  getOptionalNumber(key: string): number | undefined;
  // (undocumented)
  getOptionalString(key: string): string | undefined;
  // (undocumented)
  getOptionalStringArray(key: string): string[] | undefined;
  // (undocumented)
  getString(key: string): string;
  // (undocumented)
  getStringArray(key: string): string[];
  // (undocumented)
  has(key: string): boolean;
  // (undocumented)
  keys(): string[];
}

// Warning: (ae-missing-release-tag) "JsonArray" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export interface JsonArray extends Array<JsonValue> {}

// Warning: (ae-missing-release-tag) "JsonObject" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export type JsonObject = {
  [key in string]?: JsonValue;
};

// Warning: (ae-missing-release-tag) "JsonPrimitive" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export type JsonPrimitive = number | string | boolean | null;

// Warning: (ae-missing-release-tag) "JsonValue" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export type JsonValue = JsonObject | JsonArray | JsonPrimitive;

// (No @packageDocumentation comment for this package)
```
