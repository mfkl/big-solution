```
msbuild Dense.sln /t:build /logger:FileLogger,Microsoft.Build.Engine;logfile=perf.log;encoding=Unicode;performancesummary
```

```
Target Performance Summary:
        * ms  Build                                      1 calls
        0 ms  _CopySourceItemsToOutputDirectory        100 calls
        0 ms  Compile                                  100 calls
        0 ms  AddSourceRevisionToInformationalVersion  100 calls
        0 ms  AfterResGen                              100 calls
        0 ms  PrepareResourceNames                     100 calls
        0 ms  CoreBuild                                100 calls
        0 ms  ValidateProjects                           1 calls
        0 ms  InitializeSourceControlInformation       100 calls
        0 ms  BeforeResolveReferences                  100 calls
        0 ms  BeforeCompile                            100 calls
        0 ms  GenerateAssemblyInfo                     100 calls
        0 ms  SetWin32ManifestProperties               100 calls
        0 ms  ValidateToolsVersions                      1 calls
        0 ms  AfterBuild                               100 calls
        0 ms  ResGen                                   100 calls
        0 ms  PrepareForRun                            100 calls
        0 ms  AfterCompile                             100 calls
        0 ms  PrepareResources                         100 calls
        0 ms  GetFrameworkPaths                        100 calls
        0 ms  BeforeBuild                              100 calls
        0 ms  PrepareProjectReferences                 100 calls
        1 ms  _CheckForObsoleteDotNetCliToolReferences 100 calls
        1 ms  CreateSatelliteAssemblies                100 calls
        1 ms  CreateCustomManifestResourceNames        100 calls
        1 ms  ResolvePackageDependenciesForBuild       100 calls
        1 ms  BeforeResGen                             100 calls
        2 ms  ResolveSDKReferences                     100 calls
        2 ms  _GetProjectJsonPath                      100 calls
        2 ms  ExpandSDKReferences                      100 calls
        2 ms  ResolveLockFileAnalyzers                 100 calls
        2 ms  ComputeRunAnalyzers                      100 calls
        2 ms  _CheckForLanguageAndFeatureCombinationSupport 100 calls
        3 ms  GetReferenceAssemblyPaths                100 calls
        5 ms  _CheckForUnsupportedCppNETCoreVersion    100 calls
        5 ms  _CheckForUnsupportedNETStandardVersion   100 calls
        5 ms  IncludeTransitiveProjectReferences       100 calls
        5 ms  _ComputePackageReferencePublish          100 calls
        6 ms  GetTargetPath                            100 calls
        6 ms  BuildOnlySettings                        100 calls
        7 ms  AfterResolveReferences                   100 calls
        7 ms  _DefaultMicrosoftNETPlatformLibrary      100 calls
        9 ms  _PopulateCommonStateForGetCopyToOutputDirectoryItems 100 calls
       11 ms  EnableIntermediateOutputPathMismatchWarning 100 calls
       11 ms  CollectPackageReferences                 100 calls
       11 ms  GetNativeManifest                         99 calls
       12 ms  GetTargetPathWithTargetPlatformMoniker   100 calls
       14 ms  ComputePackageRoots                      100 calls
       15 ms  ResolveLockFileCopyLocalFiles            100 calls
       16 ms  _GenerateCompileInputs                   100 calls
       16 ms  GetTargetFrameworks                       99 calls
       19 ms  _GetCopyToOutputDirectoryItemsFromThisProject 100 calls
       19 ms  CollectFSharpDesignTimeTools             100 calls
       20 ms  ValidateSolutionConfiguration              1 calls
       23 ms  GetAssemblyAttributes                    100 calls
       27 ms  _CollectTargetFrameworkForTelemetry      100 calls
       28 ms  ResolveReferences                        100 calls
       28 ms  CoreResGen                               100 calls
       33 ms  PrepareForBuild                          100 calls
       34 ms  ApplyImplicitVersions                    100 calls
       35 ms  _CheckForCompileOutputs                  100 calls
       36 ms  CheckForDuplicateItems                   100 calls
       41 ms  _GenerateSatelliteAssemblyInputs         100 calls
       44 ms  CheckForImplicitPackageReferenceOverrides 100 calls
       45 ms  SplitResourcesByCulture                  100 calls
       49 ms  _GetRestoreProjectStyle                  100 calls
       50 ms  _SetEmbeddedWin32ManifestProperties      100 calls
       52 ms  AssignTargetPaths                        100 calls
       53 ms  _CheckForInvalidConfigurationAndPlatform 100 calls
       54 ms  GetAssemblyVersion                       100 calls
       82 ms  GenerateFSharpTextResources              100 calls
      147 ms  _ComputeUserRuntimeAssemblies            100 calls
      202 ms  ResolvePackageAssets                     100 calls
      215 ms  _HandlePackageFileConflicts              100 calls
      247 ms  _GetFrameworkAssemblyReferences          100 calls
      266 ms  CreateGeneratedAssemblyInfoInputsCacheFile 100 calls
      293 ms  AssignProjectConfiguration               100 calls
      313 ms  IncrementalClean                         100 calls
      318 ms  _ComputeReferenceAssemblies              100 calls
      332 ms  CopyFilesToOutputDirectory               100 calls
      348 ms  ResolveLockFileReferences                100 calls
      440 ms  GenerateBuildDependencyFile              100 calls
      461 ms  RedirectFSharpCoreReferenceToNewRedistributableLocation 100 calls
      610 ms  RedirectTPReferenceToNewRedistributableLocation 100 calls
      867 ms  _CleanGetCurrentAndPriorFileWrites       100 calls
     1103 ms  _SplitProjectReferencesByFileExistence   100 calls
     1476 ms  CoreGenerateAssemblyInfo                 100 calls
     1932 ms  FindReferenceAssembliesForReferences     100 calls
     2386 ms  _CopyFilesMarkedCopyLocal                 99 calls
     2518 ms  CoreCompile                              100 calls
     3723 ms  GenerateTargetFrameworkMonikerAttribute  100 calls
     6531 ms  _GetCopyToOutputDirectoryItemsFromTransitiveProjectReferences 100 calls
     6652 ms  GetCopyToOutputDirectoryItems            100 calls
     7493 ms  ResolveProjectReferences                 100 calls
     7546 ms  _GetProjectReferenceTargetFrameworkProperties 100 calls
    14344 ms  ResolveAssemblyReferences                100 calls
        (* = timing was not recorded because of reentrancy)

Task Performance Summary:
        * ms  MSBuild                                    1 calls
        1 ms  Telemetry                                100 calls
        5 ms  FindAppConfigFile                        100 calls
        5 ms  GetFrameworkPath                         100 calls
        8 ms  FSharpEmbedResourceText                  100 calls
       10 ms  Delete                                   100 calls
       14 ms  CheckForImplicitPackageReferenceOverrides 100 calls
       15 ms  AssignCulture                            100 calls
       15 ms  CheckForDuplicateItems                   300 calls
       19 ms  GetRestoreProjectStyleTask               100 calls
       19 ms  ApplyImplicitVersions                    100 calls
       28 ms  AssignTargetPath                         600 calls
       28 ms  FSharpEmbedResXSource                    100 calls
       33 ms  MakeDir                                  200 calls
       34 ms  GetAssemblyVersion                       100 calls
       75 ms  ConvertToAbsolutePath                    100 calls
       82 ms  ReadLinesFromFile                        100 calls
      101 ms  WriteLinesToFile                         100 calls
      107 ms  ResolvePackageFileConflicts              100 calls
      110 ms  RemoveDuplicates                         200 calls
      112 ms  JoinItems                                100 calls
      123 ms  Hash                                     100 calls
      157 ms  ResolvePackageAssets                     100 calls
      186 ms  Message                                  301 calls
      198 ms  AssignProjectConfiguration               100 calls
      290 ms  FindUnderPath                            500 calls
      316 ms  GetReferenceNearestTargetFrameworkTask    99 calls
      589 ms  Touch                                     99 calls
     1817 ms  Copy                                     299 calls
     6607 ms  CallTarget                               200 calls
    14228 ms  ResolveAssemblyReference                 100 calls
        (* = timing was not recorded because of reentrancy)

Build succeeded.
    0 Warning(s)
    0 Error(s)

Time Elapsed 00:01:01.14
```