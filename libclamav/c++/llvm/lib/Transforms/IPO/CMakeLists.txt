add_llvm_library(LLVMipo
  ArgumentPromotion.cpp
  ConstantMerge.cpp
  DeadArgumentElimination.cpp
  DeadTypeElimination.cpp
  ExtractGV.cpp
  FunctionAttrs.cpp
  GlobalDCE.cpp
  GlobalOpt.cpp
  IPConstantPropagation.cpp
  IPO.cpp
  InlineAlways.cpp
  InlineSimple.cpp
  Inliner.cpp
  Internalize.cpp
  LoopExtractor.cpp
  LowerSetJmp.cpp
  MergeFunctions.cpp
  PartialInlining.cpp
  PartialSpecialization.cpp
  PruneEH.cpp
  StripDeadPrototypes.cpp
  StripSymbols.cpp
  StructRetPromotion.cpp
  )

target_link_libraries (LLVMipo LLVMScalarOpts LLVMInstCombine)
