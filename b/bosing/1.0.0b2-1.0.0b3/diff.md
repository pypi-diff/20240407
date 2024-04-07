# Comparing `tmp/bosing-1.0.0b2.tar.gz` & `tmp/bosing-1.0.0b3.tar.gz`

## Comparing `bosing-1.0.0b2.tar` & `bosing-1.0.0b3.tar`

### file list

```diff
@@ -1,129 +1,129 @@
--rw-r--r--   0        0        0    17327 2020-02-02 00:00:00.000000 bosing-1.0.0b2/.editorconfig
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 bosing-1.0.0b2/.gitattributes
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 bosing-1.0.0b2/.readthedocs.yaml
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 bosing-1.0.0b2/Bosing.sln
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bosing-1.0.0b2/Directory.Build.props
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bosing-1.0.0b2/VERSION.txt
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 bosing-1.0.0b2/WaveGenBenchmarks.EnvelopeCacheBench-report-github.md
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 bosing-1.0.0b2/WaveGenBenchmarks.WaveformUtilsBench-report-github.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bosing-1.0.0b2/exclusion.dic
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 bosing-1.0.0b2/.github/dependabot.yml
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 bosing-1.0.0b2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 bosing-1.0.0b2/examples/WaveGenBenchmarks/EnvelopeCacheBench.cs
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 bosing-1.0.0b2/examples/WaveGenBenchmarks/Program.cs
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 bosing-1.0.0b2/examples/WaveGenBenchmarks/WaveGenBenchmarks.csproj
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 bosing-1.0.0b2/examples/WaveGenBenchmarks/WaveformUtilsBench.cs
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 bosing-1.0.0b2/python/bosing/__init__.py
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 bosing-1.0.0b2/python/bosing/_native.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 bosing-1.0.0b2/python/bosing/_utils.py
--rw-r--r--   0        0        0    17757 2020-02-02 00:00:00.000000 bosing-1.0.0b2/python/bosing/models.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bosing-1.0.0b2/python/docs/Makefile
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 bosing-1.0.0b2/python/docs/api.rst
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 bosing-1.0.0b2/python/docs/conf.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 bosing-1.0.0b2/python/docs/index.rst
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 bosing-1.0.0b2/python/docs/instruction.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 bosing-1.0.0b2/python/docs/make.bat
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 bosing-1.0.0b2/python/docs/quickstart.rst
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 bosing-1.0.0b2/python/docs/requirements.txt
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 bosing-1.0.0b2/python/docs/schedule.rst
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 bosing-1.0.0b2/python/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 bosing-1.0.0b2/python/docs/_templates/autosummary/module.rst
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 bosing-1.0.0b2/python/example/schedule.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 bosing-1.0.0b2/python/example/schedule_stress.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bosing-1.0.0b2/python/tests/test_basic.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/BiquadChain.cs
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/BiquadCoefficients.cs
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/BiquadFilter.cs
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Bosing.csproj
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/BosingOptions.cs
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/ComplexReadOnlySpan.cs
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/ComplexSpan.cs
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Envelope.cs
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/EnvelopeCacheKey.cs
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/EnvelopeInfo.cs
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/EnvelopeSample.cs
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/FirCoefficients.cs
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/HannPulseShape.cs
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/IPulseShape.cs
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/InterpolatedPulseShape.cs
--rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/IqPair.cs
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/MathUtils.cs
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/PhaseTrackingTransform.cs
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/PooledComplexArray.cs
--rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/PostProcessTransform.cs
--rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/PulseList.cs
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/SignalFilter.cs
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/TimeAxisUtils.cs
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/TrianglePulseShape.cs
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/ValueArray.cs
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/WaveformSampler.cs
--rw-r--r--   0        0        0    29862 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/WaveformUtils.cs
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Schedules/AbsoluteSchedule.cs
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Schedules/Alignment.cs
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Schedules/ArrangeOption.cs
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Schedules/BarrierElement.cs
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Schedules/GridLength.cs
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Schedules/GridLengthUnit.cs
--rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Schedules/GridSchedule.cs
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Schedules/PlayElement.cs
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Schedules/RepeatElement.cs
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Schedules/Schedule.cs
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Schedules/ScheduleElement.cs
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Schedules/SetFrequencyElement.cs
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Schedules/SetPhaseElement.cs
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Schedules/ShiftFrequencyElement.cs
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Schedules/ShiftPhaseElement.cs
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Schedules/StackSchedule.cs
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Schedules/SwapPhaseElement.cs
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing/Schedules/Thickness.cs
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Api.cs
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Bosing.Aot.csproj
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/ScheduleRunner.cs
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/UnsafeMemoryManager.cs
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/AbsoluteScheduleDto.cs
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/BarrierElementDto.cs
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/BiquadDto.cs
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/ChannelInfo.cs
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/GridScheduleDto.cs
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/HannShapeInfo.cs
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/InterpolatedShapeInfo.cs
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/IqCalibration.cs
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/OptionsDto.cs
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/PlayElementDto.cs
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/RepeatElementDto.cs
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/ScheduleElementDto.cs
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/ScheduleRequest.cs
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/SetFrequencyElementDto.cs
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/SetPhaseElementDto.cs
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/ShapeInfo.cs
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/ShiftFrequencyElementDto.cs
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/ShiftPhaseElementDto.cs
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/StackScheduleDto.cs
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 bosing-1.0.0b2/src/Bosing.Aot/Models/SwapPhaseElementDto.cs
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/Bosing.Tests.csproj
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/ComplexReadOnlySpanTests.cs
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/EnvelopeInfoTests.cs
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/HannPulseShapeTests.cs
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/IntegrationTests.cs
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/IqPairTests.cs
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/MathUtilsTests.cs
--rw-r--r--   0        0        0     7704 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/PooledComplexArrayTests.cs
--rw-r--r--   0        0        0     6888 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/PulseListTests.cs
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/TimeAxisUtilsTests.cs
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/ToleranceComparer.cs
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/TrianglePulseShapeTests.cs
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/Usings.cs
--rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/WaveformUtilsTests.cs
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/Schedules/AbsoluteScheduleTests.cs
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/Schedules/FakeScheduleElement.cs
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/Schedules/GridScheduleTests.cs
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/Schedules/RepeatElementTests.cs
--rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/Schedules/ScheduleElementTests.cs
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/Schedules/ScheduleTests.cs
--rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 bosing-1.0.0b2/tests/Bosing.Tests/Schedules/StackScheduleTests.cs
--rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 bosing-1.0.0b2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 bosing-1.0.0b2/LICENSE.txt
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 bosing-1.0.0b2/README.md
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 bosing-1.0.0b2/hatch_build.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 bosing-1.0.0b2/pyproject.toml
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 bosing-1.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0    17327 2020-02-02 00:00:00.000000 bosing-1.0.0b3/.editorconfig
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 bosing-1.0.0b3/.gitattributes
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 bosing-1.0.0b3/.readthedocs.yaml
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 bosing-1.0.0b3/Bosing.sln
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bosing-1.0.0b3/Directory.Build.props
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bosing-1.0.0b3/VERSION.txt
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 bosing-1.0.0b3/WaveGenBenchmarks.EnvelopeCacheBench-report-github.md
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 bosing-1.0.0b3/WaveGenBenchmarks.WaveformUtilsBench-report-github.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bosing-1.0.0b3/exclusion.dic
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 bosing-1.0.0b3/.github/dependabot.yml
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 bosing-1.0.0b3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 bosing-1.0.0b3/examples/WaveGenBenchmarks/EnvelopeCacheBench.cs
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 bosing-1.0.0b3/examples/WaveGenBenchmarks/Program.cs
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 bosing-1.0.0b3/examples/WaveGenBenchmarks/WaveGenBenchmarks.csproj
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 bosing-1.0.0b3/examples/WaveGenBenchmarks/WaveformUtilsBench.cs
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/bosing/__init__.py
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/bosing/_native.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/bosing/_utils.py
+-rw-r--r--   0        0        0    18568 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/bosing/models.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/Makefile
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/api.rst
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/conf.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/index.rst
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/instruction.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/make.bat
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/quickstart.rst
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/requirements.txt
+-rw-r--r--   0        0        0     5572 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/schedule.rst
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/example/schedule.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/example/schedule_stress.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/tests/test_basic.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/BiquadChain.cs
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/BiquadCoefficients.cs
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/BiquadFilter.cs
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Bosing.csproj
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/BosingOptions.cs
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/ComplexReadOnlySpan.cs
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/ComplexSpan.cs
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Envelope.cs
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/EnvelopeCacheKey.cs
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/EnvelopeInfo.cs
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/EnvelopeSample.cs
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/FirCoefficients.cs
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/HannPulseShape.cs
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/IPulseShape.cs
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/InterpolatedPulseShape.cs
+-rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/IqPair.cs
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/MathUtils.cs
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/PhaseTrackingTransform.cs
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/PooledComplexArray.cs
+-rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/PostProcessTransform.cs
+-rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/PulseList.cs
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/SignalFilter.cs
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/TimeAxisUtils.cs
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/TrianglePulseShape.cs
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/ValueArray.cs
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/WaveformSampler.cs
+-rw-r--r--   0        0        0    29862 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/WaveformUtils.cs
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/AbsoluteSchedule.cs
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/Alignment.cs
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/ArrangeOption.cs
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/BarrierElement.cs
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/GridLength.cs
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/GridLengthUnit.cs
+-rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/GridSchedule.cs
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/PlayElement.cs
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/RepeatElement.cs
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/Schedule.cs
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/ScheduleElement.cs
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/SetFrequencyElement.cs
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/SetPhaseElement.cs
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/ShiftFrequencyElement.cs
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/ShiftPhaseElement.cs
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/StackSchedule.cs
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/SwapPhaseElement.cs
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/Thickness.cs
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Api.cs
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Bosing.Aot.csproj
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/ScheduleRunner.cs
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/UnsafeMemoryManager.cs
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/AbsoluteScheduleDto.cs
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/BarrierElementDto.cs
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/BiquadDto.cs
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/ChannelInfo.cs
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/GridScheduleDto.cs
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/HannShapeInfo.cs
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/InterpolatedShapeInfo.cs
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/IqCalibration.cs
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/OptionsDto.cs
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/PlayElementDto.cs
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/RepeatElementDto.cs
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/ScheduleElementDto.cs
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/ScheduleRequest.cs
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/SetFrequencyElementDto.cs
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/SetPhaseElementDto.cs
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/ShapeInfo.cs
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/ShiftFrequencyElementDto.cs
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/ShiftPhaseElementDto.cs
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/StackScheduleDto.cs
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/SwapPhaseElementDto.cs
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/Bosing.Tests.csproj
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/ComplexReadOnlySpanTests.cs
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/EnvelopeInfoTests.cs
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/HannPulseShapeTests.cs
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/IntegrationTests.cs
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/IqPairTests.cs
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/MathUtilsTests.cs
+-rw-r--r--   0        0        0     7704 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/PooledComplexArrayTests.cs
+-rw-r--r--   0        0        0     6888 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/PulseListTests.cs
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/TimeAxisUtilsTests.cs
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/ToleranceComparer.cs
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/TrianglePulseShapeTests.cs
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/Usings.cs
+-rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/WaveformUtilsTests.cs
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/Schedules/AbsoluteScheduleTests.cs
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/Schedules/FakeScheduleElement.cs
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/Schedules/GridScheduleTests.cs
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/Schedules/RepeatElementTests.cs
+-rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/Schedules/ScheduleElementTests.cs
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/Schedules/ScheduleTests.cs
+-rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/Schedules/StackScheduleTests.cs
+-rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 bosing-1.0.0b3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 bosing-1.0.0b3/LICENSE.txt
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 bosing-1.0.0b3/README.md
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 bosing-1.0.0b3/hatch_build.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 bosing-1.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 bosing-1.0.0b3/PKG-INFO
```

### Comparing `bosing-1.0.0b2/.editorconfig` & `bosing-1.0.0b3/.editorconfig`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/.gitattributes` & `bosing-1.0.0b3/.gitattributes`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/.readthedocs.yaml` & `bosing-1.0.0b3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/Bosing.sln` & `bosing-1.0.0b3/Bosing.sln`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/WaveGenBenchmarks.EnvelopeCacheBench-report-github.md` & `bosing-1.0.0b3/WaveGenBenchmarks.EnvelopeCacheBench-report-github.md`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/WaveGenBenchmarks.WaveformUtilsBench-report-github.md` & `bosing-1.0.0b3/WaveGenBenchmarks.WaveformUtilsBench-report-github.md`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/.github/workflows/ci.yml` & `bosing-1.0.0b3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/examples/WaveGenBenchmarks/EnvelopeCacheBench.cs` & `bosing-1.0.0b3/examples/WaveGenBenchmarks/EnvelopeCacheBench.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/examples/WaveGenBenchmarks/WaveformUtilsBench.cs` & `bosing-1.0.0b3/examples/WaveGenBenchmarks/WaveformUtilsBench.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/python/bosing/__init__.py` & `bosing-1.0.0b3/python/bosing/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 """Generates microwave pulses for superconducting quantum computing experiments.
 
-This module wraps the ``Bosing`` C# library.
+.. caution::
 
-.. note::
-    All phase values are in number of cycles. For example, a phase of 0.25 means
-    pi/2 radians.
-
-.. warning::
-    This package is still in development and the API may change in the future.
+    All phase values are in number of cycles. For example, a phase of
+    :math:`0.25` means :math:`\\pi/2` radians.
 """
 
 from ._utils import generate_waveforms
 from .models import (
     Absolute,
     AbsoluteEntry,
     Alignment,
@@ -20,15 +16,15 @@
     Channel,
     Element,
     Grid,
     GridEntry,
     GridLength,
     Hann,
     Interp,
-    IqCalibration,
+    IqCali,
     Options,
     Play,
     Repeat,
     SetFreq,
     SetPhase,
     ShiftFreq,
     ShiftPhase,
@@ -41,15 +37,15 @@
     "Alignment",
     "Barrier",
     "Biquad",
     "Channel",
     "Grid",
     "Hann",
     "Interp",
-    "IqCalibration",
+    "IqCali",
     "Options",
     "Play",
     "Repeat",
     "SetFreq",
     "SetPhase",
     "ShiftFreq",
     "ShiftPhase",
```

### Comparing `bosing-1.0.0b2/python/bosing/_native.py` & `bosing-1.0.0b3/python/bosing/_native.py`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/python/bosing/_utils.py` & `bosing-1.0.0b3/python/bosing/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import typing
 
 import numpy as np
 
 from ._native import copy_waveform, free_waveform, run
-from .models import Channel, Element, Options, Request, ShapeInfo
+from .models import Channel, Element, Options, Request, Shape
 
 
 def generate_waveforms(
     channels: typing.Iterable[Channel],
-    shapes: typing.Iterable[ShapeInfo],
+    shapes: typing.Iterable[Shape],
     schedule: Element,
     options: typing.Optional[Options] = None,
 ) -> typing.Dict[str, typing.Tuple[np.ndarray, np.ndarray]]:
-    """Generate waveforms for the given request.
+    """Generate waveforms.
 
     :param channels: Information about the channels used in the schedule.
     :param shapes: Information about the shapes used in the schedule.
     :param schedule: The root element of the schedule.
-    :param options: Options for the Bosing service.
+    :param options: Various options for the waveform generation.
     :return: A dictionary of waveforms, where the key is the channel name and
         the value is a tuple of two numpy arrays representing the I and Q
         components of the waveform.
     """
     request = Request(
         channels=channels,
         shapes=shapes,
```

### Comparing `bosing-1.0.0b2/python/bosing/models.py` & `bosing-1.0.0b3/python/bosing/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 class UnionObject(MsgObject):
     """Base class for all union objects.
 
     A union object is a message object that can be one of several types.
     """
 
     TYPE_ID: _typing.ClassVar[int]
-    """The type ID of the union object."""
 
     @property
     def data(self) -> tuple:
         return (self.TYPE_ID, super().data)
 
 
 @_attrs.frozen
@@ -58,65 +57,65 @@
     b1: float
     b2: float
     a1: float
     a2: float
 
 
 @_attrs.frozen
-class IqCalibration(MsgObject):
+class IqCali(MsgObject):
     """IQ calibration data.
 
     The calibration data consists of a 2x2 transformation matrix and an 2x1 offset
     vector. The transformation matrix is applied first, followed by the offset vector.
 
     .. math::
-        \\begin{bmatrix}
+        \\begin{pmatrix}
             I_{out} \\\\
             Q_{out}
-        \\end{bmatrix} =
-        \\begin{bmatrix}
+        \\end{pmatrix} =
+        \\begin{pmatrix}
             a & b \\\\
             c & d
-        \\end{bmatrix}
-        \\begin{bmatrix}
+        \\end{pmatrix}
+        \\begin{pmatrix}
             I_{in} \\\\
             Q_{in}
-        \\end{bmatrix} +
-        \\begin{bmatrix}
+        \\end{pmatrix} +
+        \\begin{pmatrix}
             i_{offset} \\\\
             q_{offset}
-        \\end{bmatrix}
+        \\end{pmatrix}
     """
 
     a: float
     b: float
     c: float
     d: float
     i_offset: float = 0
     q_offset: float = 0
 
 
 @_attrs.frozen
 class Channel(MsgObject):
-    """Information about a channel."""
+    """Channel configuration."""
 
     name: str
     base_freq: float
     sample_rate: float
-    delay: float
     length: int
+    delay: float = 0
     align_level: int = -10
-    iq_calibration: _typing.Optional[IqCalibration] = None
+    iq_calibration: _typing.Optional[IqCali] = None
     iir: _typing.List[Biquad] = _attrs.field(factory=list, converter=list)
     fir: _typing.List[float] = _attrs.field(factory=list, converter=list)
 
 
 @_attrs.frozen
 class Options(MsgObject):
-    """Options for Bosing.
+    """Various options for waveform generation.
 
     :param time_tolerance: The time tolerance of the scheduler.
     :param amp_tolerance: The amplitude tolerance in waveform calculation.
     :param phase_tolerance: The phase tolerance in waveform calculation.
     :param allow_oversize: Whether to allow arranging schedules with duration shorter than desired.
     """
 
@@ -126,19 +125,16 @@
     allow_oversize: bool = False
 
 
 class Alignment(_enum.Enum):
     """Alignment of a schedule element."""
 
     END = 0
-    """Align to the end of parent element."""
     START = 1
-    """Align to the start of parent element."""
     CENTER = 2
-    """Align to the center of parent element."""
     STRETCH = 3
     """Stretch to fill parent element."""
 
 
 def _convert_margin(
     margin: _typing.Union[float, _typing.Tuple[float, float]]
 ) -> _typing.Tuple[float, float]:
@@ -154,51 +150,62 @@
 ) -> Alignment:
     if isinstance(alignment, str):
         return Alignment[alignment.upper()]
     return alignment
 
 
 @_attrs.frozen
-class ShapeInfo(UnionObject):
-    """Information about a shape."""
+class Shape(UnionObject):
+    """Base class for shapes."""
 
 
 @_attrs.frozen
-class Hann(ShapeInfo):
+class Hann(Shape):
     """A Hann shape."""
 
     TYPE_ID = 0
 
 
 @_attrs.frozen
-class Interp(ShapeInfo):
+class Interp(Shape):
     """An interpolated shape."""
 
     TYPE_ID = 1
 
     x_array: _typing.List[float] = _attrs.field(converter=list)
     y_array: _typing.List[float] = _attrs.field(converter=list)
 
 
 @_attrs.frozen
 class Element(UnionObject):
     """Base class for schedule elements.
 
     A schedule element is a node in the tree structure of a schedule similar to
-    HTML elements. The design is inspired by `XAML in WPF / WinUI <https://learn.
-    microsoft.com/en-us/windows/apps/design/layout/layouts-with-xaml>`_
+    HTML elements. The design is inspired by `XAML in WPF / WinUI
+    <https://learn.microsoft.com/en-us/windows/apps/design/layout/layouts-with-xaml>`_
+
+    When :attr:`duration`, :attr:`max_duration`, and :attr:`min_duration` are
+    conflicting, the priority is as follows:
+
+    1. :attr:`min_duration`
+    2. :attr:`max_duration`
+    3. :attr:`duration`
 
     :param margin: The margin of the element. If a single value is given, it is
-        used for both sides.
+        used for both sides. Default to 0.
     :type margin: float | tuple[float, float]
-    :param alignment: The alignment of the element.
-    :param visibility: Whether the element has effect on the output.
-    :param duration: Requested duration of the element.
-    :param max_duration: Maximum duration of the element.
-    :param min_duration: Minimum duration of the element.
+    :param alignment: The alignment of the element. Default to
+        :attr:`Alignment.END`.
+    :param visibility: Whether the element has effect on the output. Default to
+        ``True``.
+    :param duration: Requested duration of the element. If ``None``, the actual
+        duration is determined by the measuring and arranging process. Default
+        to ``None``.
+    :param max_duration: Maximum duration of the element. Default to infinity.
+    :param min_duration: Minimum duration of the element. Default to 0.
     """
 
     margin: _typing.Tuple[float, float] = _attrs.field(
         kw_only=True, default=(0, 0), converter=_convert_margin
     )
     alignment: Alignment = _attrs.field(
         kw_only=True, default=Alignment.END, converter=_convert_alignment
@@ -210,26 +217,28 @@
 
 
 @_attrs.frozen
 class Play(Element):
     """A pulse play element.
 
     If :attr:`flexible` is set to ``True`` and :attr:`alignment` is set to
-    :attr:`Alignment.STRETCH`, the duration of the pulse is determined by the
-    parent element such as :class:`Grid`.
+    :attr:`Alignment.STRETCH`, the plateau of the pulse is stretched to fill the
+    parent element.
 
     :param channel_id: Target channel ID.
     :param amplitude: The amplitude of the pulse.
     :param shape_id: The shape ID of the pulse.
     :param width: The width of the pulse.
-    :param plateau: The plateau of the pulse.
-    :param drag_coef: The drag coefficient of the pulse.
-    :param frequency: The frequency of the pulse.
-    :param phase: The phase of the pulse in **cycles**.
-    :param flexible: Whether the pulse can be shortened or extended.
+    :param plateau: The plateau of the pulse. Default to 0.
+    :param drag_coef: The drag coefficient of the pulse. Default to 0.
+    :param frequency: Additional frequency of the pulse on top of channel base
+        frequency and frequency shift. Default to 0.
+    :param phase: Additional phase of the pulse in **cycles**. Default to 0.
+    :param flexible: Whether the pulse can be shortened or extended. Default to
+        ``False``.
     """
 
     TYPE_ID = 0
 
     channel_id: int
     amplitude: float
     shape_id: int
@@ -255,16 +264,24 @@
     phase: float
 
 
 @_attrs.frozen
 class SetPhase(Element):
     """A phase set element.
 
-    Currently the effect of set phase instruction is calculated based on the
-    cumulative frequency shift. This may change in the future.
+    Given the base frequency :math:`f`, the frequency shift :math:`\\Delta f`,
+    the time :math:`t`, and the phase offset :math:`\\phi_0`, the phase is
+    defined as
+
+    .. math::
+
+        \\phi(t) = (f + \\Delta f) t + \\phi_0
+
+    :class:`SetPhase` sets the phase offset :math:`\\phi_0` such that
+    :math:`\\phi(t)` is equal to the given phase.
 
     :param channel_id: Target channel ID.
     :param phase: Target phase in **cycles**.
     """
 
     TYPE_ID = 2
 
@@ -272,54 +289,57 @@
     phase: float
 
 
 @_attrs.frozen
 class ShiftFreq(Element):
     """A frequency shift element.
 
+    Additional frequency shift on top of the channel cumulative frequency shift.
+    Phase offset will be adjusted accordingly such that the phase is continuous
+    at the shift point.
+
     :param channel_id: Target channel ID.
     :param frequency: Delta frequency.
     """
 
     TYPE_ID = 3
 
     channel_id: int
     frequency: float
 
 
 @_attrs.frozen
 class SetFreq(Element):
     """A frequency set element.
 
+    Set the channel frequency shift to the target frequency. Phase offset will
+    be adjusted accordingly such that the phase is continuous at the shift point.
+
     :param channel_id: Target channel ID.
     :param frequency: Target frequency.
     """
 
     TYPE_ID = 4
 
     channel_id: int
     frequency: float
 
 
 @_attrs.frozen
 class SwapPhase(Element):
     """A phase swap element.
 
-    Let :math:`\\phi_1` and :math:`\\phi_2` be the phases of the two target
-    channels, respectively. The effect of the swap phase instruction is to
-    change the phases to :math:`\\phi_2` and :math:`\\phi_1`, respectively.
-    Currently the phase :math:`\\phi` is defined as
+    This instruction swaps carrier phases between two target channels at the
+    scheduled time point. Carrier phase is defined as
 
     .. math::
-        \\phi = (f + \\Delta f) t + \\phi_0
+        \\phi(t) = (f + \\Delta f) t + \\phi_0
 
-    where :math:`f` is the frequency defined in
-    :class:`bosing.models.Channel`, :math:`\\Delta f` is the
-    frequency shift due to :class:`ShiftFreq`, and :math:`\\phi_0` is the
-    phase offset due to :class:`ShiftPhase` and other phase instructions.
+    where :math:`f` is the base frequency, :math:`\\Delta f` is the frequency
+    shift, :math:`t` is the time, and :math:`\\phi_0` is the phase offset.
 
     :param channel_id1: Target channel ID 1.
     :param channel_id2: Target channel ID 2.
     """
 
     TYPE_ID = 5
 
@@ -333,29 +353,29 @@
 
     A barrier element is a zero-duration no-op element. Useful for aligning
     elements on different channels in :class:`Stack`.
 
     If :attr:`channel_ids` is empty, the barrier is applied to
     all channels in its parent element.
 
-    :param channel_ids: Target channel IDs.
+    :param channel_ids: Target channel IDs. Default to empty.
     """
 
     TYPE_ID = 6
 
     channel_ids: _typing.List[int] = _attrs.field(converter=list, factory=list)
 
 
 @_attrs.frozen
 class Repeat(Element):
     """A repeated schedule element.
 
     :param child: The repeated element.
     :param count: The number of repetitions.
-    :param spacing: The spacing between repeated elements.
+    :param spacing: The spacing between repeated elements. Default to 0.
     """
 
     TYPE_ID = 7
 
     child: Element
     count: int
     spacing: float = _attrs.field(kw_only=True, default=0)
@@ -379,16 +399,18 @@
 
 
 @_attrs.frozen
 class Stack(Element):
     """Layout child elements in one direction.
 
     The child elements are arranged in one direction. The direction can be
-    forwards or backwards. :class:`Barrier` can be used to synchronize
-    multiple channels.
+    forwards or backwards.
+
+    Child elements with no common channel are arranged in parallel.
+    :class:`Barrier` can be used to synchronize multiple channels.
 
     :param children: Child elements.
     :param direction: The direction of arrangement.
     """
 
     TYPE_ID = 8
 
@@ -637,14 +659,14 @@
 @_attrs.frozen
 class Request(MsgObject):
     """A schedule request.
 
     :param channels: Information about the channels used in the schedule.
     :param shapes: Information about the shapes used in the schedule.
     :param schedule: The root element of the schedule.
-    :param options: Options for the Bosing service.
+    :param options: Various options for waveform generation.
     """
 
     channels: _typing.List[Channel] = _attrs.field(converter=list)
-    shapes: _typing.List[ShapeInfo] = _attrs.field(converter=list)
+    shapes: _typing.List[Shape] = _attrs.field(converter=list)
     schedule: Element
     options: Options = _attrs.field(factory=Options)
```

### Comparing `bosing-1.0.0b2/python/docs/Makefile` & `bosing-1.0.0b3/python/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/python/docs/conf.py` & `bosing-1.0.0b3/python/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/python/docs/make.bat` & `bosing-1.0.0b3/python/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/python/docs/schedule.rst` & `bosing-1.0.0b3/python/docs/schedule.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,149 +1,173 @@
-Schedule API
-============
+波形编排
+========
 
 .. currentmodule:: bosing.models
 
-Schedule API 使用类似 HTML、XAML 的结构来描述波形序列，用户可以定义基础的波形，然后通过组合的方式来构建复杂的波形序列。基础元素有 :doc:`instruction`：
+``bosing`` 使用类似 HTML, XAML 的结构来描述波形序列, 用户可以定义基础的波形,
+然后通过组合的方式来构建复杂的波形序列. 基础元素有 :doc:`instruction`:
 
 * :class:`Play`
 * :class:`ShiftPhase`
 * :class:`SetPhase`
 * :class:`ShiftFreq`
 * :class:`SetFreq`
 * :class:`SwapPhase`
 
-另外还有：
+另外还有:
 
 * :class:`Repeat`
-    根据指定的次数与间隔重复子元素
+    根据指定的次数与间隔重复子元素.
 
 * :class:`Barrier`
-    用于在 :class:`Stack` 中同步多个通道
+    用于在 :class:`Stack` 中同步多个通道.
 
-以及布局容器：
+以及布局容器:
 
 * :class:`Stack`
-    将多个元素按照顺序排列，类似于 `Stack Layout <https://learn.microsoft.com/en-us/dotnet/maui/user-interface/layouts/stacklayout>`_，应该是最常用的容器
+    将多个元素按照顺序排列, 类似于 `Stack Layout
+    <https://learn.microsoft.com/en-us/dotnet/maui/user-interface/layouts/stacklayout>`_,
+    应该是最常用的容器.
 
 * :class:`Absolute`
-    指定子元素相对于容器的绝对时间，类似于 `Absolute Layout <https://learn.microsoft.com/en-us/dotnet/maui/user-interface/layouts/absolutelayout>`_
+    指定子元素相对于容器的绝对时间, 类似于 `Absolute Layout
+    <https://learn.microsoft.com/en-us/dotnet/maui/user-interface/layouts/absolutelayout>`_.
 
 * :class:`Grid`
-    按照定义的 column 宽度排列子元素，类似于 `Grid Layout <https://learn.microsoft.com/en-us/dotnet/maui/user-interface/layouts/grid>`_
+    按照定义的 column 宽度排列子元素, 类似于 `Grid Layout
+    <https://learn.microsoft.com/en-us/dotnet/maui/user-interface/layouts/grid>`_.
 
 
 基础属性
 --------
 
-每个元素都有以下基础属性：
+每个元素都有以下基础属性:
 
 :attr:`Element.margin`
-    元素前后额外占用的时间，默认为 ``0``
+    元素前后额外占用的时间, 默认为 ``0``.
 
 :attr:`Element.visibility`
-    元素是否生效，如果为 ``False`` 虽然会占用布局空间，但是不会执行相应指令
+    元素是否生效, 如果为 ``False`` 虽然会占用布局空间, 但是不会执行相应指令.
 
 :attr:`Element.alignment`
-    元素在容器中的对齐方式，目前只有 :class:`Grid` 会使用该属性，其他布局会忽略该属性
+    元素在容器中的对齐方式, 目前只有 :class:`Grid` 会使用该属性, 其他布局会忽略
+    该属性.
 
 :attr:`Element.duration`
-    元素的持续时间，默认为 ``None``，由布局系统根据子元素计算
+    元素的持续时间, 默认为 ``None``, 由布局系统根据子元素计算.
 
 :attr:`Element.max_duration`
-    元素的最大持续时间，默认为 ``inf``
+    元素的最大持续时间, 默认为 ``inf``.
 
 :attr:`Element.min_duration`
-    元素的最小持续时间，默认为 ``0``
+    元素的最小持续时间, 默认为 ``0``.
 
 .. note::
 
-    布局系统参考的是 XAML 的方案，相邻元素的 ``margin`` 不会重叠。例如，如果两个相邻元素的 ``margin`` 分别为 ``0.1`` 和 ``0.2``，那么它们之间的间隔为 ``0.3`` 而不是 ``0.2``。
+    布局系统参考的是 XAML 的方案, 相邻元素的 ``margin`` 不会重叠. 例如, 如果两个
+    相邻元素的 ``margin`` 分别为 ``0.1`` 和 ``0.2``, 那么它们之间的间隔为
+    ``0.3`` 而不是 ``0.2``.
 
 .. note::
 
-    GUI 布局中如果子元素的大小超过了容器的大小，布局系统会裁剪子元素。但是在波形计算中，往往需要保留子元素的完整波形，因此一旦出现超出容器的情况会抛出异常。
+    GUI 布局中如果子元素的大小超过了容器的大小, 布局系统会裁剪子元素. 但是在波形
+    计算中, 往往需要保留子元素的完整波形, 因此一旦出现超出容器的情况会抛出异常.
 
 .. note:: 
 
-    当 :attr:`Element.duration`、:attr:`Element.max_duration`、:attr:`Element.min_duration` 三个属性同时存在且存在冲突时，优先级为 ``min_duration > max_duration > duration``
+    当 :attr:`Element.duration`, :attr:`Element.max_duration`,
+    :attr:`Element.min_duration` 三个属性同时存在且存在冲突时, 优先级为
+    ``min_duration > max_duration > duration``.
 
 
 Stack 布局
 ----------
 
-在保持子元素前后顺序不变的前提下，按照 :attr:`Stack.direction` 指定的方向排列子元素，默认为 :attr:`ArrangeDirection.BACKWARDS`，子元素尽量靠后排列。如果需要同步多个通道，可以使用 :class:`Barrier`。子元素的 :attr:`Element.alignment` 属性会被忽略，持续时间尽可能短。
+在保持子元素前后顺序不变的前提下, 按照 :attr:`Stack.direction` 指定的方向排列子
+元素, 默认为 :attr:`ArrangeDirection.BACKWARDS`, 子元素尽量靠后排列. 如果需要同
+步多个通道, 可以使用 :class:`Barrier`. 子元素的 :attr:`Element.alignment` 属性会
+被忽略, 持续时间尽可能短.
 
 
 Absolute 布局
 -------------
 
-可以指定子元素相对于容器起点的位置。子元素的 :attr:`Element.alignment` 属性会被忽略，持续时间尽可能短。子元素的位置非负，容器的持续时间记录为起点到最晚结束的子元素的终点。
+可以指定子元素相对于容器起点的位置. 子元素的 :attr:`Element.alignment` 属性会被
+忽略, 持续时间尽可能短. 子元素的位置非负, 容器的持续时间记录为起点到最晚结束的子
+元素的终点.
 
-添加子元素时需要指定位置，默认为 ``0``
+添加子元素时需要指定位置, 默认为 ``0``.
 
 .. code-block:: python
 
     absolute = Absolute().with_children(
         Play(...),
         (1e-9, Play(...)),
         (2e-9, Stack(...)),
     )
 
 
 Grid 布局
 ---------
 
-将容器内部划分为若干列，每个子元素占据单列或多列，允许多个子元素占据同一列。计算完固定长度与 ``Auto`` 长度的列后，剩余的长度会按比例分配给 ``Star`` 长度的列。子元素在列内部按照 :attr:`Element.alignment` 属性指定的方式排列。可以利用该布局实现居中对齐的效果，还可以配合 :attr:`Play.flexible` 实现根据子元素的持续时间自动调整背景波形持续时间的效果。
+将容器内部划分为若干列, 每个子元素占据单列或多列, 允许多个子元素占据同一列. 计算
+完固定长度与 ``Auto`` 长度的列后, 剩余的长度会按比例分配给 ``Star`` 长度的列. 子
+元素在列内部按照 :attr:`Element.alignment` 属性指定的方式排列. 可以利用该布局实
+现居中对齐的效果, 还可以配合 :attr:`Play.flexible` 实现根据子元素的持续时间自动
+调整背景波形持续时间的效果.
 
-添加子元素时需要指定列，默认为 ``0``，以及跨列数，默认为 ``1``，如果超出了容器的列数会当作最后一列处理。
+添加子元素时需要指定列, 默认为 ``0``, 以及跨列数, 默认为 ``1``, 如果超出了容器的
+列数会当作最后一列处理.
 
 .. code-block:: python
 
     grid = Grid(columns=["*", "*", "*"]).with_children(
         Play(...),
         (1, Play(...)),
         (0, 3, Stack(...)),
     )
 
 .. tip::
 
-    指定 column 宽度时，可以使用 ``"Auto"``、``"*"``、``"2*"`` 等形式
+    指定 column 宽度时, 可以使用 ``"Auto"``, ``"*"``, ``"2*"`` 等形式.
 
     .. code-block:: python
 
         grid = Grid(columns=["Auto", "*", "2*", 30e-9])
 
 .. caution:: 
 
-    当可用时长较小时，无法保证按比例分配 ``Star`` 长度的列。
+    当可用时长较小时, 无法保证按比例分配 ``Star`` 长度的列.
 
 
 布局算法
 --------
 
-布局过程分为两步：
+布局过程分为两步:
 
-1. Measure 阶段：给定可用空间，计算每个元素的最小持续时间。最顶层的容器的可用空间为 ``inf``，子元素的可用空间由父元素决定。
-2. Arrange 阶段：根据 Measure 阶段计算出的持续时间，计算每个元素相对于父元素的位置。如果提供的可用空间不足，会抛出异常。
+1. Measure 阶段: 给定可用空间, 计算每个元素的最小持续时间. 最顶层的容器的可用空
+   间为 ``inf``, 子元素的可用空间由父元素决定.
+2. Arrange 阶段: 根据 Measure 阶段计算出的持续时间, 计算每个元素相对于父元素的位
+   置. 如果提供的可用空间不足, 会抛出异常.
 
-使用时可以给最顶层的容器指定 :attr:`Element.duration`，限制布局的持续时间。
+使用时可以给最顶层的容器指定 :attr:`Element.duration`, 限制布局的持续时间.
 
 
 执行顺序
 --------
 
 .. caution:: 
 
-    在布局完成后，会按照子元素插入顺序遍历执行，与布局得到的元素位置无关。
+    在布局完成后, 会按照子元素插入顺序遍历执行, 与布局得到的元素位置无关.
 
 
 波形对齐
 --------
 
-程序在采样包络时会对波形进行对齐，即将波形的起始点对齐到某个单位时间的整数倍。对齐参数在 :attr:`Channel.align_level` 中指定，假设给定值为 :math:`n`，采样间隔为 :math:`\Delta t`，则对齐的单位时间为 :math:`2^n\Delta t`，比如 ``align_level`` 为 -4，则单位时间为 :math:`2^{-4}\Delta t`，即 :math:`\Delta t / 16`。
+程序在采样包络时会对波形进行对齐, 即将波形的起始点对齐到某个单位时间的整数倍. 对
+齐参数在 :attr:`Channel.align_level` 中指定, 假设给定值为 :math:`n`, 采样间隔为
+:math:`\Delta t`, 则对齐的单位时间为 :math:`2^n\Delta t`, 比如 ``align_level``
+为 -4, 则单位时间为 :math:`2^{-4}\Delta t`, 即 :math:`\Delta t / 16`.
 
+.. note::
 
-计算结果
---------
-
-目前程序会返回一个字典，键为通道名，值为一个元组，元组中的第一个元素为 I 通道的采样值，第二个元素为 Q 通道的采样值。
+    波形对齐目前主要是为了便于重用缓存波形.
```

### Comparing `bosing-1.0.0b2/python/docs/_templates/autosummary/module.rst` & `bosing-1.0.0b3/python/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/python/example/schedule.py` & `bosing-1.0.0b3/python/example/schedule.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,38 +17,34 @@
     k = 1 + amp
     z, p, k = signal.bilinear_zpk([z], [p], k, fs)
     sos = signal.zpk2sos(p, z, 1 / k)
     return Biquad(sos[0][0], sos[0][1], sos[0][2], sos[0][4], sos[0][5])
 
 
 def get_iq_calibration(ratio, phase, offset_i, offset_q):
-    return IqCalibration(
-        1, -math.tan(phase), 0, ratio / math.cos(phase), offset_i, offset_q
-    )
+    return IqCali(1, -math.tan(phase), 0, ratio / math.cos(phase), offset_i, offset_q)
 
 
 if __name__ == "__main__":
     t0 = perf_counter()
 
     bq = get_biquad(-0.1, 20e-9, 2e9)
     fir = signal.firwin(5, 100e6, fs=2e9)
     channels = [
         Channel(
             "xy0",
             0,
             2e9,
-            0,
             100000,
-            -10,
             iq_calibration=get_iq_calibration(1.1, math.pi / 3, 0, 0),
         ),
-        Channel("xy1", 0, 2e9, 0, 100000, -10),
-        Channel("u0", 0, 2e9, 0, 100000, -10, iir=[bq]),
-        Channel("u1", 0, 2e9, 0, 100000, -10, iir=[bq], fir=fir),
-        Channel("m0", 0, 2e9, 0, 100000, 0),
+        Channel("xy1", 0, 2e9, 100000),
+        Channel("u0", 0, 2e9, 100000, iir=[bq]),
+        Channel("u1", 0, 2e9, 100000, iir=[bq], fir=fir),
+        Channel("m0", 0, 2e9, 100000),
     ]
     c = {ch.name: i for i, ch in enumerate(channels)}
     halfcos = np.sin(np.linspace(0, np.pi, 10))
     shapes = [
         Hann(),
         Interp(np.linspace(-0.5, 0.5, 10), halfcos),
     ]
```

### Comparing `bosing-1.0.0b2/python/example/schedule_stress.py` & `bosing-1.0.0b3/python/example/schedule_stress.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 def gen_n(n: int):
     t0 = time.perf_counter()
     nxy = 64
     nu = 2 * nxy
     nm = nxy // 8
     channels = (
-        [Channel(f"xy{i}", 3e6 * i, 2e9, 0, 100000, -10) for i in range(nxy)]
-        + [Channel(f"u{i}", 0, 2e9, 0, 100000, -10) for i in range(nu)]
-        + [Channel(f"m{i}", 0, 2e9, 0, 100000, 0) for i in range(nm)]
+        [Channel(f"xy{i}", 3e6 * i, 2e9, 100000) for i in range(nxy)]
+        + [Channel(f"u{i}", 0, 2e9, 100000) for i in range(nu)]
+        + [Channel(f"m{i}", 0, 2e9, 100000) for i in range(nm)]
     )
     c = {ch.name: i for i, ch in enumerate(channels)}
     halfcos = np.sin(np.linspace(0, np.pi, 10))
     shapes = [
         Hann(),
         Interp(np.linspace(-0.5, 0.5, 10), halfcos),
     ]
```

### Comparing `bosing-1.0.0b2/python/tests/test_basic.py` & `bosing-1.0.0b3/python/tests/test_basic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 
 import bosing
 
 
 def test_basic():
-    channels = [bosing.Channel("xy0", 100e6, 2e9, 0, 100000, -10)]
+    channels = [bosing.Channel("xy0", 100e6, 2e9, 100000)]
     shapes = [bosing.Hann()]
     schedule = bosing.Stack(duration=49.9e-6).with_children(
         bosing.Play(0, 0.1, 0, 100e-9)
     )
     result = bosing.generate_waveforms(channels, shapes, schedule)
     assert "xy0" in result
     i, q = result["xy0"]
```

### Comparing `bosing-1.0.0b2/src/Bosing/BiquadChain.cs` & `bosing-1.0.0b3/src/Bosing/BiquadChain.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/BiquadCoefficients.cs` & `bosing-1.0.0b3/src/Bosing/BiquadCoefficients.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/BiquadFilter.cs` & `bosing-1.0.0b3/src/Bosing/BiquadFilter.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/Bosing.csproj` & `bosing-1.0.0b3/src/Bosing/Bosing.csproj`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/BosingOptions.cs` & `bosing-1.0.0b3/src/Bosing/BosingOptions.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/ComplexReadOnlySpan.cs` & `bosing-1.0.0b3/src/Bosing/ComplexReadOnlySpan.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/ComplexSpan.cs` & `bosing-1.0.0b3/src/Bosing/ComplexSpan.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/Envelope.cs` & `bosing-1.0.0b3/src/Bosing/Envelope.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/EnvelopeInfo.cs` & `bosing-1.0.0b3/src/Bosing/EnvelopeInfo.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/EnvelopeSample.cs` & `bosing-1.0.0b3/src/Bosing/EnvelopeSample.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/FirCoefficients.cs` & `bosing-1.0.0b3/src/Bosing/FirCoefficients.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/HannPulseShape.cs` & `bosing-1.0.0b3/src/Bosing/HannPulseShape.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/IPulseShape.cs` & `bosing-1.0.0b3/src/Bosing/IPulseShape.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/InterpolatedPulseShape.cs` & `bosing-1.0.0b3/src/Bosing/InterpolatedPulseShape.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/IqPair.cs` & `bosing-1.0.0b3/src/Bosing/IqPair.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/MathUtils.cs` & `bosing-1.0.0b3/src/Bosing/MathUtils.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/PhaseTrackingTransform.cs` & `bosing-1.0.0b3/src/Bosing/PhaseTrackingTransform.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/PooledComplexArray.cs` & `bosing-1.0.0b3/src/Bosing/PooledComplexArray.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/PostProcessTransform.cs` & `bosing-1.0.0b3/src/Bosing/PostProcessTransform.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/PulseList.cs` & `bosing-1.0.0b3/src/Bosing/PulseList.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/SignalFilter.cs` & `bosing-1.0.0b3/src/Bosing/SignalFilter.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/TimeAxisUtils.cs` & `bosing-1.0.0b3/src/Bosing/TimeAxisUtils.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/ValueArray.cs` & `bosing-1.0.0b3/src/Bosing/ValueArray.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/WaveformSampler.cs` & `bosing-1.0.0b3/src/Bosing/WaveformSampler.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/WaveformUtils.cs` & `bosing-1.0.0b3/src/Bosing/WaveformUtils.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/Schedules/AbsoluteSchedule.cs` & `bosing-1.0.0b3/src/Bosing/Schedules/AbsoluteSchedule.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/Schedules/BarrierElement.cs` & `bosing-1.0.0b3/src/Bosing/Schedules/BarrierElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/Schedules/GridLength.cs` & `bosing-1.0.0b3/src/Bosing/Schedules/GridLength.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/Schedules/GridSchedule.cs` & `bosing-1.0.0b3/src/Bosing/Schedules/GridSchedule.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/Schedules/PlayElement.cs` & `bosing-1.0.0b3/src/Bosing/Schedules/PlayElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/Schedules/RepeatElement.cs` & `bosing-1.0.0b3/src/Bosing/Schedules/RepeatElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/Schedules/Schedule.cs` & `bosing-1.0.0b3/src/Bosing/Schedules/Schedule.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/Schedules/ScheduleElement.cs` & `bosing-1.0.0b3/src/Bosing/Schedules/ScheduleElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/Schedules/SetFrequencyElement.cs` & `bosing-1.0.0b3/src/Bosing/Schedules/SetFrequencyElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/Schedules/SetPhaseElement.cs` & `bosing-1.0.0b3/src/Bosing/Schedules/SetPhaseElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/Schedules/ShiftFrequencyElement.cs` & `bosing-1.0.0b3/src/Bosing/Schedules/ShiftFrequencyElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/Schedules/ShiftPhaseElement.cs` & `bosing-1.0.0b3/src/Bosing/Schedules/ShiftPhaseElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/Schedules/StackSchedule.cs` & `bosing-1.0.0b3/src/Bosing/Schedules/StackSchedule.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing/Schedules/SwapPhaseElement.cs` & `bosing-1.0.0b3/src/Bosing/Schedules/SwapPhaseElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing.Aot/Api.cs` & `bosing-1.0.0b3/src/Bosing.Aot/Api.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing.Aot/Bosing.Aot.csproj` & `bosing-1.0.0b3/src/Bosing.Aot/Bosing.Aot.csproj`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing.Aot/ScheduleRunner.cs` & `bosing-1.0.0b3/src/Bosing.Aot/ScheduleRunner.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing.Aot/Models/AbsoluteScheduleDto.cs` & `bosing-1.0.0b3/src/Bosing.Aot/Models/AbsoluteScheduleDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing.Aot/Models/BarrierElementDto.cs` & `bosing-1.0.0b3/src/Bosing.Aot/Models/BarrierElementDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing.Aot/Models/BiquadDto.cs` & `bosing-1.0.0b3/src/Bosing.Aot/Models/BiquadDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing.Aot/Models/GridScheduleDto.cs` & `bosing-1.0.0b3/src/Bosing.Aot/Models/GridScheduleDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing.Aot/Models/OptionsDto.cs` & `bosing-1.0.0b3/src/Bosing.Aot/Models/OptionsDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing.Aot/Models/PlayElementDto.cs` & `bosing-1.0.0b3/src/Bosing.Aot/Models/PlayElementDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing.Aot/Models/RepeatElementDto.cs` & `bosing-1.0.0b3/src/Bosing.Aot/Models/RepeatElementDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing.Aot/Models/ScheduleElementDto.cs` & `bosing-1.0.0b3/src/Bosing.Aot/Models/ScheduleElementDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing.Aot/Models/SetFrequencyElementDto.cs` & `bosing-1.0.0b3/src/Bosing.Aot/Models/SetFrequencyElementDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing.Aot/Models/SetPhaseElementDto.cs` & `bosing-1.0.0b3/src/Bosing.Aot/Models/SetPhaseElementDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing.Aot/Models/ShiftFrequencyElementDto.cs` & `bosing-1.0.0b3/src/Bosing.Aot/Models/ShiftFrequencyElementDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing.Aot/Models/ShiftPhaseElementDto.cs` & `bosing-1.0.0b3/src/Bosing.Aot/Models/ShiftPhaseElementDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing.Aot/Models/StackScheduleDto.cs` & `bosing-1.0.0b3/src/Bosing.Aot/Models/StackScheduleDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/src/Bosing.Aot/Models/SwapPhaseElementDto.cs` & `bosing-1.0.0b3/src/Bosing.Aot/Models/SwapPhaseElementDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/tests/Bosing.Tests/Bosing.Tests.csproj` & `bosing-1.0.0b3/tests/Bosing.Tests/Bosing.Tests.csproj`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/tests/Bosing.Tests/ComplexReadOnlySpanTests.cs` & `bosing-1.0.0b3/tests/Bosing.Tests/ComplexReadOnlySpanTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/tests/Bosing.Tests/EnvelopeInfoTests.cs` & `bosing-1.0.0b3/tests/Bosing.Tests/EnvelopeInfoTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/tests/Bosing.Tests/HannPulseShapeTests.cs` & `bosing-1.0.0b3/tests/Bosing.Tests/HannPulseShapeTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/tests/Bosing.Tests/IntegrationTests.cs` & `bosing-1.0.0b3/tests/Bosing.Tests/IntegrationTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/tests/Bosing.Tests/IqPairTests.cs` & `bosing-1.0.0b3/tests/Bosing.Tests/IqPairTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/tests/Bosing.Tests/PooledComplexArrayTests.cs` & `bosing-1.0.0b3/tests/Bosing.Tests/PooledComplexArrayTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/tests/Bosing.Tests/PulseListTests.cs` & `bosing-1.0.0b3/tests/Bosing.Tests/PulseListTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/tests/Bosing.Tests/TimeAxisUtilsTests.cs` & `bosing-1.0.0b3/tests/Bosing.Tests/TimeAxisUtilsTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/tests/Bosing.Tests/TrianglePulseShapeTests.cs` & `bosing-1.0.0b3/tests/Bosing.Tests/TrianglePulseShapeTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/tests/Bosing.Tests/WaveformUtilsTests.cs` & `bosing-1.0.0b3/tests/Bosing.Tests/WaveformUtilsTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/tests/Bosing.Tests/Schedules/AbsoluteScheduleTests.cs` & `bosing-1.0.0b3/tests/Bosing.Tests/Schedules/AbsoluteScheduleTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/tests/Bosing.Tests/Schedules/FakeScheduleElement.cs` & `bosing-1.0.0b3/tests/Bosing.Tests/Schedules/FakeScheduleElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/tests/Bosing.Tests/Schedules/GridScheduleTests.cs` & `bosing-1.0.0b3/tests/Bosing.Tests/Schedules/GridScheduleTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/tests/Bosing.Tests/Schedules/RepeatElementTests.cs` & `bosing-1.0.0b3/tests/Bosing.Tests/Schedules/RepeatElementTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/tests/Bosing.Tests/Schedules/ScheduleElementTests.cs` & `bosing-1.0.0b3/tests/Bosing.Tests/Schedules/ScheduleElementTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/tests/Bosing.Tests/Schedules/ScheduleTests.cs` & `bosing-1.0.0b3/tests/Bosing.Tests/Schedules/ScheduleTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/tests/Bosing.Tests/Schedules/StackScheduleTests.cs` & `bosing-1.0.0b3/tests/Bosing.Tests/Schedules/StackScheduleTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/.gitignore` & `bosing-1.0.0b3/.gitignore`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/LICENSE.txt` & `bosing-1.0.0b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/hatch_build.py` & `bosing-1.0.0b3/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b2/pyproject.toml` & `bosing-1.0.0b3/pyproject.toml`

 * *Files identical despite different names*

